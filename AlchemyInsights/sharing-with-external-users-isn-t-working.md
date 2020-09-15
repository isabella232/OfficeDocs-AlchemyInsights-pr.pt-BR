---
title: O compartilhamento com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691563"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="edcf9-102">Corrigir problemas de compartilhamento de conteúdo do SharePoint com usuários externos</span><span class="sxs-lookup"><span data-stu-id="edcf9-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="edcf9-103">Certifique-se de que o compartilhamento externo está ativado para sua organização:</span><span class="sxs-lookup"><span data-stu-id="edcf9-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="edcf9-104">Vá até a [ &amp; página suplementos de serviços no centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="edcf9-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="edcf9-105">Certifique-se de que a configuração está ativada para "ativado".</span><span class="sxs-lookup"><span data-stu-id="edcf9-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="edcf9-106">Se "somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="edcf9-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="edcf9-107">Verifique se o compartilhamento externo está ativado para o site.</span><span class="sxs-lookup"><span data-stu-id="edcf9-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="edcf9-108">Para um conjunto de sites clássico:</span><span class="sxs-lookup"><span data-stu-id="edcf9-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="edcf9-109">No novo centro de administração do SharePoint, no painel esquerdo, clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="edcf9-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="edcf9-110">Selecione o site ou sites e, na faixa de opções, clique em **compartilhamento**.</span><span class="sxs-lookup"><span data-stu-id="edcf9-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="edcf9-111">Para um site de equipe que pertença a um grupo do Microsoft 365 ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="edcf9-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="edcf9-112">Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração em toda a organização, a menos que a configuração em toda a organização permita o compartilhamento de arquivos usando links que não exigem logon.</span><span class="sxs-lookup"><span data-stu-id="edcf9-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="edcf9-113">Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entram.</span><span class="sxs-lookup"><span data-stu-id="edcf9-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="edcf9-114">Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="edcf9-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="edcf9-115">[Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="edcf9-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="edcf9-116">A configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="edcf9-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

