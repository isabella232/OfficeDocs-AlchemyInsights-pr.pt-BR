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
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="22904-102">Corrigindo os aplicativos do Office "não é possível estabelecer uma conexão agora"</span><span class="sxs-lookup"><span data-stu-id="22904-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="22904-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="22904-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="22904-104">Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="22904-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="22904-105">Confira [URLs e intervalos de endereços IP da Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="22904-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="22904-106">Vá para **Iniciar** > **executar**e digite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="22904-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="22904-107">Certifique-se de que os seguintes serviços estejam em execução:</span><span class="sxs-lookup"><span data-stu-id="22904-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="22904-108">Configuração automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="22904-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="22904-109">Serviço de lista de rede</span><span class="sxs-lookup"><span data-stu-id="22904-109">Network List Service</span></span>
    - <span data-ttu-id="22904-110">Reconhecimento de local de rede</span><span class="sxs-lookup"><span data-stu-id="22904-110">Network Location Awareness</span></span>
    - <span data-ttu-id="22904-111">Log de eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="22904-111">Windows Event Log</span></span>

<span data-ttu-id="22904-112">Se um desses serviços não estiver em execução, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="22904-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="22904-113">Se você tiver problemas para iniciar o serviço, execute o seguinte comando abrindo um prompt de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="22904-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="22904-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="22904-114">**sfc /scannow**</span></span>

<span data-ttu-id="22904-115">Após a conclusão desse comando, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="22904-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="22904-116">Para obter informações detalhadas, consulte ["não é possível conectar-se à sua conta. Tente novamente mais tarde "quando você ativar o Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="22904-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>