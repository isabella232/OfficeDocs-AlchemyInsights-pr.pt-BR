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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744583"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Corrigindo Microsoft 365 de aplicativos "Não podemos nos conectar agora" mensagem

Observação: se você estiver usando uma versão mais antiga do Windows (por exemplo, Windows 7 SP1, Windows Server [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 2008 R2), use a correção fácil para habilitar o TLS 1.2 como padrão. Para obter mais informações, confira [Atualizar para habilitar o TLS 1.1 e o TLS 1.2 como os protocolos seguros padrão em WinHTTP no Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

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