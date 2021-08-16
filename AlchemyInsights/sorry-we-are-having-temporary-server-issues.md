---
title: Corrigindo Microsoft 365 aplicativos Desculpe, estamos tendo problemas temporários de servidor mensagem
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021584"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigir os Microsoft 365 aplicativos "Desculpe, estamos tendo problemas temporários de servidor" mensagem

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para Microsoft 365 aplicativos. Consulte [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar**  >  **Executar** e digite **services.msc**. Certifique-se de que os seguintes serviços estão em execução:
    - Instalação automática de dispositivos conectados à rede
    - Serviço de Lista de Rede
    - Reconhecimento de Localização de Rede
    - Windows Log de Eventos

Se um desses serviços não estiver em execução, tente in inicie-lo. Se você tiver um problema ao iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc /scannow**

Depois que esse comando terminar, reinicie o computador.

Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Tente novamente mais tarde" erro quando você ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).