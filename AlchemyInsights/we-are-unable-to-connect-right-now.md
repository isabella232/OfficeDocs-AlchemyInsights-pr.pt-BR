---
title: Problema de ativação - Não podemos nos conectar agora
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998134"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Corrigindo Microsoft 365 de aplicativos "Não podemos nos conectar agora" mensagem

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para Microsoft 365 aplicativos. Consulte [URLs da Microsoft e intervalos de endereços IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Vá para **Iniciar**  >  **Executar** e digite **services.msc**. Certifique-se de que os seguintes serviços estão em execução:
    - Instalação automática de dispositivos conectados à rede
    - Serviço de Lista de Rede
    - Reconhecimento de Localização de Rede
    - Windows Log de Eventos

Se um desses serviços não estiver em execução, tente in inicie-lo. Se você tiver um problema ao iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc /scannow**

Depois que esse comando terminar, reinicie o computador.

Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Tente novamente mais tarde" quando você](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)ativar Office de Microsoft 365 .