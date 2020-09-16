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
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="417af-102">Corrigindo os aplicativos do Microsoft 365 "não é possível estabelecer uma conexão com o momento"</span><span class="sxs-lookup"><span data-stu-id="417af-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="417af-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="417af-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="417af-104">Verifique as configurações de firewall, software antivírus e proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="417af-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="417af-105">Confira [URLs e intervalos de endereços IP da Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="417af-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="417af-106">Vá para **Iniciar**  >  **executar**e digite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="417af-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="417af-107">Certifique-se de que os seguintes serviços estejam em execução:</span><span class="sxs-lookup"><span data-stu-id="417af-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="417af-108">Configuração automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="417af-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="417af-109">Serviço de lista de rede</span><span class="sxs-lookup"><span data-stu-id="417af-109">Network List Service</span></span>
    - <span data-ttu-id="417af-110">Reconhecimento de local de rede</span><span class="sxs-lookup"><span data-stu-id="417af-110">Network Location Awareness</span></span>
    - <span data-ttu-id="417af-111">Log de eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="417af-111">Windows Event Log</span></span>

<span data-ttu-id="417af-112">Se um desses serviços não estiver em execução, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="417af-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="417af-113">Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="417af-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="417af-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="417af-114">**sfc /scannow**</span></span>

<span data-ttu-id="417af-115">Após a conclusão desse comando, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="417af-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="417af-116">Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "quando você ativar o Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="417af-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>