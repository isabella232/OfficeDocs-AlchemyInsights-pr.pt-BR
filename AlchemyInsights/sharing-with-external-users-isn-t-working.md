---
title: O compartilhamento com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207673"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="fe14f-102">Corrigir problemas de compartilhamento de conteúdo do SharePoint com usuários externos</span><span class="sxs-lookup"><span data-stu-id="fe14f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="fe14f-103">Certifique-se de que o compartilhamento externo está ativado para sua organização:</span><span class="sxs-lookup"><span data-stu-id="fe14f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="fe14f-104">Vá até a [página &amp; suplementos de serviços no centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="fe14f-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="fe14f-p101">Certifique-se de que a configuração está ativada para "ativado". Se "somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fe14f-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="fe14f-p102">Verifique se o compartilhamento externo está ativado para o site. Para um conjunto de sites clássico:</span><span class="sxs-lookup"><span data-stu-id="fe14f-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="fe14f-109">No centro de administração do SharePoint clássico, no painel esquerdo, clique em **conjuntos de sites**.</span><span class="sxs-lookup"><span data-stu-id="fe14f-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="fe14f-110">Selecione o site ou sites e, na faixa de opções, clique em **compartilhamento**.</span><span class="sxs-lookup"><span data-stu-id="fe14f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="fe14f-111">Para um site de equipe que pertença a um grupo do Office 365 ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="fe14f-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="fe14f-p103">Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração em toda a organização, a menos que a configuração em toda a organização permita o compartilhamento de arquivos usando links que não exigem logon. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entram. Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint (versão prévia) ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="fe14f-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="fe14f-116">A configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="fe14f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

