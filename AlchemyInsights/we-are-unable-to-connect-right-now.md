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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716160"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Corrigindo os aplicativos do Office "não é possível estabelecer uma conexão agora"

Se você receber essa mensagem, tente o seguinte:

1. Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Office. Confira [URLs e intervalos de endereços IP da Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar** > **executar**e digite **Services. msc**. Certifique-se de que os seguintes serviços estejam em execução:
    - Configuração automática de dispositivos conectados à rede
    - Serviço de lista de rede
    - Reconhecimento de local de rede
    - Log de eventos do Windows

Se um desses serviços não estiver em execução, tente iniciá-lo. Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc/scannow**

Após a conclusão desse comando, reinicie o computador.

Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "quando você ativar o Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).