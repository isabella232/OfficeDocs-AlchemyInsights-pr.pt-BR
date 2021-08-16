---
title: Estou sendo bloqueado pelo Acesso Condicional usando um dispositivo compatível
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019136"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Estou sendo bloqueado pelo Acesso Condicional usando um dispositivo compatível

**Ferramentas Altamente Recomendadas**

- [Ferramenta De Solução de Problemas de Registro de Dispositivos](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/): uma ferramenta ampla que ajuda a solucionar os problemas mais comuns de registro de dispositivos.
- [Script da Conectividade de Registro de Dispositivos de Teste](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/): uma ferramenta usada para garantir que um dispositivo tenha acesso aos pontos de extremidade do Registro de Dispositivos na conta do sistema.
- [Script da Limpeza de Dispositivos do Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup): uma ferramenta usada para buscar e gerenciar dispositivos antigos no ambiente.

Veja alguns motivos comuns pelos quais o Acesso Condicional pode falhar em um dispositivo compatível, ou pelos quais seus usuários podem receber a mensagem **Não é possível ir daqui para lá** durante uma solicitação de entrada em um recurso organizacional.

1. **O dispositivo não está no estado de dispositivo necessário com um MDM**:

Valide que o dispositivo está registrado com um provedor MDM aprovado, como o Intune, e *marcado como compatível*. Para saber mais sobre o Intune, confira este [documento](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Para uma melhor compreensão da conformidade de dispositivo e do Intune, confira a [política de conformidade de uso para estabelecer regras para dispositivos gerenciados com o Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Se você estiver com problemas para registrar um dispositivo no Intune, encontre detalhes de solução de problemas em [Solucionar problemas de registro dispositivos na Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Para obter mais suporte do Intune, crie uma solicitação de suporte. Para isso, visite a [página Ajuda e Suporte do Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **O dispositivo não está associado à rede de organizações**:

Para ter acesso aos recursos organizacionais, o dispositivo precisa estar conectado à rede da organização, seja por conexão direta ou por uma rede privada virtual (VPN), e também associado localmente ou ao Azure Active Directory. Para associar um dispositivo de trabalho à rede da organização, confira [Associar seu dispositivo de trabalho à rede da organização](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Para registrar um dispositivo pessoal/BYOD, confira [Registrar seu dispositivo pessoal na rede da organização](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Para validar se o dispositivo se associou à rede, siga as etapas para dispositivos registrados [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered), ou para dispositivos de trabalho [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Para o escopo do problema de Conectividade de rede organizacional, siga as diretrizes abaixo:

    1. Entre no Windows usando sua conta corporativa ou de estudante, por exemplo, marcelo@contoso.com.
    2. Conecte-se à rede da organização por meio de uma VPN ou de DirectAccess.
    3. Após se conectar, pressione a **tecla do logotipo do Windows + L** para bloquear seu dispositivo.
    4. Desbloqueie seu dispositivo usando sua conta corporativa ou de estudante, e depois tente acessar o aplicativo ou o serviço com problemas novamente.

Se você vir a mensagem de erro **Não é possível ir daqui para lá**, é provável que o problema está em outro lugar.

3. **Não há suporte para o sistema operacional**:

Verifique se você está executando uma versão com suporte do sistema operacional, incluindo:

- **Windows Client**: Windows 7 ou posterior

- **Windows Server**: Windows Server 2008 R2 ou posterior

- **macOS**: macOS X ou posterior

- **Android e iOS**: versão mais recente dos sistemas operacionais móveis do Android e do iOS

4. **O navegador não é compatível**:

Encontre os navegadores com suporte abaixo. Para o suporte do Chrome com o Windows 1703 ou versões posteriores, é necessária uma extensão de Contas do Windows 10. No Microsoft Edge 85+, o usuário precisa estar conectado para passar corretamente as informações de conformidade do dispositivo. Para obter mais detalhes, confira [aqui](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Managed Browser do Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Encontre mais informações sobre a mensagem **Não é possível ir daqui para lá** e as etapas de solução de problemas [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
