---
title: Compartilhando com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274972"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="17d65-102">Corrigir problemas ao compartilhar o conteúdo do SharePoint com usuários externos</span><span class="sxs-lookup"><span data-stu-id="17d65-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="17d65-103">Certifique-se de compartilhamento externo está ativado para a sua organização:</span><span class="sxs-lookup"><span data-stu-id="17d65-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="17d65-104">Vá até o [serviços &amp; página de suplementos no Centro de administração do Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.</span><span class="sxs-lookup"><span data-stu-id="17d65-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="17d65-p101">Verifique se que a configuração está ativada para "Ligado". Se "Apenas usuários externos existentes" são selecionados, verifique se o usuário externo está listado no Centro de administração do Office 365.</span><span class="sxs-lookup"><span data-stu-id="17d65-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="17d65-p102">Certifique-se de externo compartilhá-lo ativado para o site. Para um conjunto de sites clássico:</span><span class="sxs-lookup"><span data-stu-id="17d65-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="17d65-109">No Centro de administração do SharePoint clássico, no painel esquerdo, clique em **conjuntos de sites**.</span><span class="sxs-lookup"><span data-stu-id="17d65-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="17d65-110">Selecione o site ou sites e na faixa de opções, clique em **compartilhar**.</span><span class="sxs-lookup"><span data-stu-id="17d65-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="17d65-111">Para um site de equipe que pertence a um grupo do Office 365, ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="17d65-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="17d65-p103">Esses novos tipos de site têm o compartilhamento mesmo definindo como sua configuração de toda a organização, a menos que a configuração de toda a organização permite o compartilhamento de arquivos usando links que não exigem entrar. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entram. Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint (preview) ou PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="17d65-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="17d65-116">A configuração de compartilhamento externa para qualquer site pode ser mais restritiva do que a configuração de toda a organização, mas não mais permissivo do que a configuração de toda a organização.</span><span class="sxs-lookup"><span data-stu-id="17d65-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

