---
title: Problema de ativação – não é possível se conectar no momento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725971"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Corrigindo os aplicativos do Microsoft 365 "não é possível estabelecer uma conexão com o momento"

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Microsoft 365. Confira [URLs e intervalos de endereços IP da Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar**  >  **executar**e digite **Services. msc**. Certifique-se de que os seguintes serviços estejam em execução:
    - Configuração automática de dispositivos conectados à rede
    - Serviço de lista de rede
    - Reconhecimento de local de rede
    - Log de eventos do Windows

Se um desses serviços não estiver em execução, tente iniciá-lo. Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc/scannow**

Após a conclusão desse comando, reinicie o computador.

Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "quando você ativar o Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).