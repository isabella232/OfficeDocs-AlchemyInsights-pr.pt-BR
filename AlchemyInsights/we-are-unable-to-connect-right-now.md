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
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="493fb-102">Corrigindo os aplicativos do Office "não é possível estabelecer uma conexão agora"</span><span class="sxs-lookup"><span data-stu-id="493fb-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="493fb-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="493fb-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="493fb-104">Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="493fb-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="493fb-105">Confira [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="493fb-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="493fb-106">Vá para **Iniciar** > **executar**e digite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="493fb-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="493fb-107">Certifique-se de que os seguintes serviços estejam em execução:</span><span class="sxs-lookup"><span data-stu-id="493fb-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="493fb-108">Configuração automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="493fb-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="493fb-109">Serviço de lista de rede</span><span class="sxs-lookup"><span data-stu-id="493fb-109">Network List Service</span></span>
    - <span data-ttu-id="493fb-110">Reconhecimento de local de rede</span><span class="sxs-lookup"><span data-stu-id="493fb-110">Network Location Awareness</span></span>
    - <span data-ttu-id="493fb-111">Log de eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="493fb-111">Windows Event Log</span></span>

<span data-ttu-id="493fb-112">Se um desses serviços não estiver em execução, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="493fb-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="493fb-113">Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="493fb-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="493fb-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="493fb-114">**sfc /scannow**</span></span>

<span data-ttu-id="493fb-115">Após a conclusão desse comando, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="493fb-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="493fb-116">Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "ao ativar o Office no Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="493fb-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>