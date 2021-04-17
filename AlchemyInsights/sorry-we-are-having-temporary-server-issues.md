---
title: Corrigir aplicativos do Microsoft 365 Desculpe, estamos tendo problemas temporários de servidor mensagem
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835259"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigir a mensagem aplicativos do Microsoft 365 "Desculpe, estamos tendo problemas temporários de servidor"

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para aplicativos do Microsoft 365. Consulte [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar**  >  **Executar** e digite **services.msc**. Certifique-se de que os seguintes serviços estão em execução:
    - Instalação automática de dispositivos conectados à rede
    - Serviço de Lista de Rede
    - Reconhecimento de Localização de Rede
    - Log de Eventos do Windows

Se um desses serviços não estiver em execução, tente in inicie-lo. Se você tiver um problema ao iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:

**sfc /scannow**

Depois que esse comando terminar, reinicie o computador.

Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Tente novamente mais tarde" erro quando você ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).