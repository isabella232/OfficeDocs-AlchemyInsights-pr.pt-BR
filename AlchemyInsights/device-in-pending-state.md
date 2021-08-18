---
title: Dispositivo em estado pendente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330360"
---
# <a name="device-in-pending-state"></a>Dispositivo em estado pendente

**Pré-requisitos:**

1. Se você estiver configurando registros de dispositivo pela primeira vez, verifique se você analisou Introdução ao gerenciamento de dispositivos no [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) que o orientará sobre como obter dispositivos sob o controle do Azure AD.
2. Se você estiver registrando dispositivos no Azure AD diretamente e registrando-os no Intune, você [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) precisará garantir que configurou o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o licenciamento em vigor primeiro.
3. Verifique se você está autorizado a executar operações no Azure AD e no AD local. Apenas um administrador global no Azure Active Directory pode gerenciar as configurações para registros de dispositivos. Além disso, se estiver configurando os registros automáticos no Active Directory local, você precisará ser um administrador do Active Directory e do AD FS (se aplicável).

O processo de registro de junção híbrida do Azure AD exige que os dispositivos sejam na rede corporativa. Ele também funciona por VPN, mas há algumas advertências para isso. Ouvimos que os clientes precisam de assistência para solucionar problemas do processo de registro de junção híbrida do Azure AD em circunstâncias de trabalho remotas.

**Ambiente de autenticação na nuvem (usando a sincronização de hash de senha do Azure AD ou autenticação de passagem)**

Esse fluxo de registro também é conhecido como "Sync Join".

Aqui está uma divisão do que acontece durante o processo de registro:

1. Windows 10 descobre o registro do Ponto de Conexão de Serviço (SCP) quando o usuário faz o login no dispositivo.

    1. O dispositivo tenta primeiro recuperar informações de locatário do SCP do lado do cliente no Registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, consulte [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Se falhar, o dispositivo se comunicará com o Active Directory local para obter informações de locatário do SCP. Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Observação**: recomendamos habilenciar o SCP no Active Directory e usar apenas o SCP do lado do cliente para validação inicial.

2. Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD.

    Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o [script Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 gera certificado auto-assinado e o armazena no objeto do computador no Active Directory local. Isso requer linha de visão para o Controlador de Domínio.

4. O objeto device que tem certificado é sincronizado com o Azure AD por meio do Azure AD Conexão. O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Conexão. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "**Pendente**" em Folha de dispositivo do Portal do Azure.

6. No próximo logon do usuário para Windows 10, o registro será concluído.

    **Observação**: se você estiver na VPN e logoff/logoff/logon encerrar a conectividade de domínio, você pode disparar o registro manualmente. Para isso:
    
    Emitir um prompt de administrador localmente `dsregcmd /join` ou remotamente por meio do PSExec para o computador.\
    Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para problemas comuns com o Azure Active Directory de dispositivos, consulte [Perguntas frequentes sobre dispositivos.](https://docs.microsoft.com/azure/active-directory/devices/faq)
