---
title: Solucionar problema de PRT
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571788"
---
# <a name="troubleshoot-prt-issue"></a>Solucionar problema de PRT

Para qualquer dispositivo concluir a autenticação, ele deve estar totalmente registrado e em bom estado e ser capaz de adquirir um token de atualização principal (PRT).

O processo de registro de ingresso do Azure AD híbrido exige que os dispositivos estejam em uma rede corporativa. Ele também funciona pela VPN, mas há algumas advertências para isso. Ouvimos clientes que precisam de assistência com a solução de problemas do processo de registro de ingresso do Azure AD híbrido em circunstâncias de trabalho remoto. Aqui está uma divisão do que está acontecendo, nos bastidores, durante o processo de registro.

**Ambiente de autenticação em nuvem (usando a sincronização de hash de senha ou autenticação de passagem do Azure AD)**

Esse fluxo de registro também é conhecido como "junção de sincronização".

1. O Windows 10 descobre um registro SCP quando o usuário faz logon no dispositivo.
    1. O dispositivo primeiro tenta recuperar informações do locatário do SCP do lado do cliente no registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Se ele falhar, o dispositivo se comunica com o Active Directory (AD) local para obter informações de locatário do ponto de conexão de serviço (SCP). Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> É recomendável habilitar o SCP no AD e usar somente o SCP do lado do cliente para validação inicial.

2. O Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD. Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o script de conectividade de registro do dispositivo de teste.

3. O Windows 10 gera um certificado autoassinado e o armazena no objeto computador no AD local. Isso exige uma linha de visão para o controlador de domínio.

4. Um objeto Device que tem um certificado é sincronizado com o Azure AD por meio do Azure AD Connect. O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Connect. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "pendente", em folha de dispositivo do portal do Azure.

6. No próximo login do usuário no Windows 10, o registro será concluído. 

> [!NOTE]
> Se você estiver na VPN e um processo de logon de logoff encerrar a conectividade do domínio, você pode disparar o registro manualmente:
 1. Emita um dsregcmd/Join localmente no prompt de administrador ou remotamente via PSExec para seu computador. Por exemplo, PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Para obter mais detalhes sobre problemas de União híbrida, consulte [Troubleshoot Devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
