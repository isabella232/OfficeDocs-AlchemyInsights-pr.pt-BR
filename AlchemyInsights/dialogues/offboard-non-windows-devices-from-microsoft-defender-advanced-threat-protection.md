---
title: Offboard de dispositivos que não são Windows da Proteção Avançada contra Ameaças do Microsoft Defender (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529906"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="e96e6-102">Offboard de dispositivos que não são Windows da Proteção Avançada contra Ameaças do Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="e96e6-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="e96e6-103">Veja como:</span><span class="sxs-lookup"><span data-stu-id="e96e6-103">Here's how:</span></span>

1. <span data-ttu-id="e96e6-104">Siga a documentação de terceiros para desconectar a solução de terceiros do Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="e96e6-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="e96e6-105">Do locatário do Azure Active Directory, remova permissões para a solução de terceiros:</span><span class="sxs-lookup"><span data-stu-id="e96e6-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="e96e6-106">Entre no [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="e96e6-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="e96e6-107">Selecione **Todos os serviços**  >  **aplicativos corporativos do Azure Active Directory.**  >  </span><span class="sxs-lookup"><span data-stu-id="e96e6-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="e96e6-108">Selecione o aplicativo que você gostaria de fazer offboard.</span><span class="sxs-lookup"><span data-stu-id="e96e6-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="e96e6-109">Selecione **Excluir**.</span><span class="sxs-lookup"><span data-stu-id="e96e6-109">Select **Delete**.</span></span>

<span data-ttu-id="e96e6-110">Para saber mais, confira [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="e96e6-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
