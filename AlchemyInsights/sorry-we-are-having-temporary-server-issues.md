---
title: Corrigindo os aplicativos do Microsoft 365 lamentamos, estamos com mensagens de problemas de servidor temporárias
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582691"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigindo os aplicativos do Microsoft 365 "Desculpe, estamos tendo problemas de servidor temporários"

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Microsoft 365. Confira [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar**  >  **executar**e digite **Services. msc**. Certifique-se de que os seguintes serviços estejam em execução:
    - Configuração automática de dispositivos conectados à rede
    - Serviço de lista de rede
    - Reconhecimento de local de rede
    - Log de eventos do Windows

Se um desses serviços não estiver em execução, tente iniciá-lo. Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc/scannow**

Após a conclusão desse comando, reinicie o computador.

Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "ao ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).