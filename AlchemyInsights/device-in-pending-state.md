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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652110"
---
# <a name="device-in-pending-state"></a>Dispositivo em estado pendente

**Pré-requisitos**

1. Se estiver configurando registros de dispositivo pela primeira vez, verifique se você analisou [a introdução ao gerenciamento de dispositivos no Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , que orientará você sobre como obter dispositivos sob o controle do Azure AD.
2. Se você estiver registrando dispositivos no Azure AD diretamente e registrá-los no Intune, será necessário garantir que você tenha configurado o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o [Licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) em vigor primeiro.
3. Certifique-se de que você está autorizado a executar operações no Azure AD e no AD local. Somente um administrador global no Azure AD pode gerenciar configurações de registros de dispositivos. Além disso, se você estiver configurando registros automáticos no seu Active Directory local, será necessário ser um administrador do Active Directory e do AD FS (se aplicável).

O processo de registro de ingresso do Azure AD híbrido exige que os dispositivos estejam na rede corporativa. Ele também funciona pela VPN, mas há algumas advertências para isso. Ouvimos clientes que precisam de assistência com a solução de problemas do processo de registro de ingresso do Azure AD híbrido em circunstâncias de trabalho remotas.

**Ambiente de autenticação em nuvem (usando a sincronização de hash de senha ou autenticação de passagem do Azure AD)**

Esse fluxo de registro também é conhecido como "junção de sincronização".

Veja a seguir uma análise do que acontece durante o processo de registro:

1. O Windows 10 descobre o registro do ponto de conexão de serviço (SCP) quando o usuário faz logon no dispositivo.

    1. O dispositivo primeiro tenta recuperar informações do locatário do SCP do lado do cliente no registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, consulte [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Se ele falhar, o dispositivo se comunica com o Active Directory local para obter informações de locatário do SCP. Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > É recomendável habilitar o SCP no Active Directory e usar somente o SCP do lado do cliente para validação inicial.

2. O Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD.

    Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o [script de conectividade de registro do dispositivo de teste](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. O Windows 10 gera um certificado autoassinado e o armazena no objeto computador no Active Directory local. Isso exige uma linha de visão para o controlador de domínio.

4. O objeto Device que tem o certificado é sincronizado com o Azure AD por meio do Azure AD Connect. O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Connect. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "**pendente**", em folha de dispositivo do portal do Azure.

6. No próximo login do usuário no Windows 10, o registro será concluído.

    > [!NOTE]
    > Se você estiver na VPN e o logoff/logon encerrar a conectividade do domínio, você poderá disparar o registro manualmente. Para isso:
    >
    > Emita um `dsregcmd /join` aviso local no prompt de administrador ou remotamente via PsExec para seu computador.
    >
    > Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para problemas comuns com o registro de dispositivos do Azure Active Directory, confira [perguntas frequentes sobre dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).
