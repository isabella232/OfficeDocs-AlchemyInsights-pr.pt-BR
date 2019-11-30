---
title: Problema de ativação – não é possível se conectar no momento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628230"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Corrigindo os aplicativos do Office "não é possível estabelecer uma conexão agora"

Se você receber essa mensagem, tente o seguinte:

1. Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Office. Confira [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar** > **executar**e digite **Services. msc**. Certifique-se de que os seguintes serviços estejam em execução:
    - Configuração automática de dispositivos conectados à rede
    - Serviço de lista de rede
    - Reconhecimento de local de rede
    - Log de eventos do Windows

Se um desses serviços não estiver em execução, tente iniciá-lo. Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc/scannow**

Após a conclusão desse comando, reinicie o computador.

Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "ao ativar o Office no Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).