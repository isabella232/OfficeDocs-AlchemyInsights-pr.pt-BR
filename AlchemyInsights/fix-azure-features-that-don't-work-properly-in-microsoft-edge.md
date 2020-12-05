---
title: O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576337"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="1b2c9-102">O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1b2c9-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="1b2c9-103">O Microsoft Edge tem [problemas conhecidos](https://go.microsoft.com/fwlink/?linkid=2140608) relacionados às zonas de segurança e pode afetar como os usuários do Azure fazem logon no centro de administração do Windows.</span><span class="sxs-lookup"><span data-stu-id="1b2c9-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="1b2c9-104">Se você estiver tendo problemas para usar os recursos do Azure com o Microsoft Edge, tente as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="1b2c9-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="1b2c9-105">No menu **Iniciar** , procure opções da **Internet** e selecione-a.</span><span class="sxs-lookup"><span data-stu-id="1b2c9-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="1b2c9-106">Na caixa de diálogo **Propriedades da Internet** , vá para a guia **segurança** .</span><span class="sxs-lookup"><span data-stu-id="1b2c9-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="1b2c9-107">Selecione a zona **sites confiáveis** e, em seguida, selecione o botão **sites** .</span><span class="sxs-lookup"><span data-stu-id="1b2c9-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="1b2c9-108">Na caixa de diálogo **sites confiáveis** , adicione sua URL de gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) , em seguida, selecione **fechar**.</span><span class="sxs-lookup"><span data-stu-id="1b2c9-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="1b2c9-109">Na caixa de diálogo **Propriedades da Internet** , vá para a guia **privacidade** .</span><span class="sxs-lookup"><span data-stu-id="1b2c9-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="1b2c9-110">Na seção **bloqueador de pop-ups** , selecione **configurações**.</span><span class="sxs-lookup"><span data-stu-id="1b2c9-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="1b2c9-111">Na caixa de diálogo que é aberta, adicione sua URL de gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) , em seguida, selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="1b2c9-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
