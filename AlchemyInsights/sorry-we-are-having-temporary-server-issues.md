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
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="f8c5b-102">Corrigir a mensagem aplicativos do Microsoft 365 "Desculpe, estamos tendo problemas temporários de servidor"</span><span class="sxs-lookup"><span data-stu-id="f8c5b-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="f8c5b-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f8c5b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f8c5b-104">Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para aplicativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f8c5b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f8c5b-105">Consulte [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f8c5b-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f8c5b-106">Vá para **Iniciar**  >  **Executar** e digite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="f8c5b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f8c5b-107">Certifique-se de que os seguintes serviços estão em execução:</span><span class="sxs-lookup"><span data-stu-id="f8c5b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f8c5b-108">Instalação automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="f8c5b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f8c5b-109">Serviço de Lista de Rede</span><span class="sxs-lookup"><span data-stu-id="f8c5b-109">Network List Service</span></span>
    - <span data-ttu-id="f8c5b-110">Reconhecimento de Localização de Rede</span><span class="sxs-lookup"><span data-stu-id="f8c5b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f8c5b-111">Log de Eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="f8c5b-111">Windows Event Log</span></span>

<span data-ttu-id="f8c5b-112">Se um desses serviços não estiver em execução, tente in inicie-lo.</span><span class="sxs-lookup"><span data-stu-id="f8c5b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f8c5b-113">Se você tiver um problema ao iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="f8c5b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f8c5b-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="f8c5b-114">**sfc /scannow**</span></span>

<span data-ttu-id="f8c5b-115">Depois que esse comando terminar, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="f8c5b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f8c5b-116">Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Tente novamente mais tarde" erro quando você ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f8c5b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>