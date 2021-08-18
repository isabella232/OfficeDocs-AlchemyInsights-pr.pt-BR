---
title: Solucionar problemas de PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330947"
---
# <a name="troubleshoot-prt-issue"></a>Solucionar problemas de PRT

Para que qualquer dispositivo conclua a autenticação, ele deve estar totalmente registrado e em bom estado e capaz de adquirir um Token de Atualização Principal (PRT).

O processo de registro de junção híbrida do Azure AD exige que os dispositivos sejam em uma rede corporativa. Ele também funciona por VPN, mas há algumas advertências para isso. Ouvimos clientes que precisam de assistência para solucionar problemas do processo de registro de junção híbrida do Azure AD em circunstâncias de trabalho remoto. Aqui está um detalhamento do que está acontecendo "sob o coifa" durante o processo de registro.

**Ambiente de autenticação na nuvem (usando a sincronização de hash de senha do Azure AD ou autenticação de passagem)**

Esse fluxo de registro também é conhecido como "Sync Join".

1. Windows 10 descobre um registro SCP ao fazer logor do usuário no dispositivo.
    1. O dispositivo tenta primeiro recuperar informações de locatário do SCP do lado do cliente no Registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Se ele falhar, o dispositivo se comunicará com o Active Directory (AD) local para obter informações de locatário do Ponto de Conexão de Serviço (SCP). Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

**Observação**: recomendamos habilenciar o SCP no AD e usar apenas o SCP do lado do cliente para validação inicial.

2. Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD. Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o script Test Device Registration Connectivity.

3. Windows 10 gera um certificado auto-assinado e o armazena no objeto do computador no AD local. Isso requer linha de visão para o Controlador de Domínio.

4. Um objeto de dispositivo que tem um certificado é sincronizado com o Azure AD por meio do Azure AD Conexão. O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Conexão. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "Pendente" em Folha de dispositivo do Portal do Azure.

6. No próximo logon do usuário para Windows 10, o registro será concluído. 

**Observação**: se você estiver na VPN e um processo de logoff-logoff encerrar a conectividade de domínio, você poderá disparar o registro manualmente:
 1. Emitir um dsregcmd /join localmente no prompt de administrador ou remotamente por meio do PSExec para seu computador. Por exemplo, \\ cmd win10client01 do PsExec , dsregcmd /join

 2. Para obter mais detalhes sobre problemas de Junção Híbrida, consulte [Solucionar problemas de dispositivos](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
