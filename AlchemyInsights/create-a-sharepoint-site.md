---
title: Criar um site do SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515795"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="3f325-102">Criar um site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="3f325-102">Create a SharePoint site</span></span>

<span data-ttu-id="3f325-103">Você pode ver o seguinte para obter informações sobre a criação de sites do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="3f325-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="3f325-104">[Gerenciar sites no novo centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Saiba mais sobre as opções de criação de site, incluindo como criar um site clássico ou um site de equipe que não inclui um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3f325-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="3f325-105">[Criar um site de equipe no SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): saiba como criar um site de equipe.</span><span class="sxs-lookup"><span data-stu-id="3f325-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="3f325-106">[Criar um site de comunicação no SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): saiba como criar um site de comunicações.</span><span class="sxs-lookup"><span data-stu-id="3f325-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="3f325-107">[Gerenciar sites no novo centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): saiba como criar um site clássico ou um site de equipe que não inclua um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3f325-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="3f325-108">[! Sobre</span><span class="sxs-lookup"><span data-stu-id="3f325-108">[!Tips]</span></span>
> - <span data-ttu-id="3f325-109">Não é possível criar um site com a mesma URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="3f325-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="3f325-110">Se você excluiu um site e deseja usar novamente a URL, é possível que o site excluído ainda exista em **sites excluídos**.</span><span class="sxs-lookup"><span data-stu-id="3f325-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="3f325-111">Para gerenciar sites excluídos, consulte [excluir um site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="3f325-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="3f325-112">Para remover completamente um site com PowerShell, consulte o exemplo do cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="3f325-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="3f325-113">Alguns usuários podem não conseguir criar um site.</span><span class="sxs-lookup"><span data-stu-id="3f325-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="3f325-114">Confira [gerenciar a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3f325-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="3f325-115">É possível que o site pareça estar preso na **criação** de mais tempo do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="3f325-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="3f325-116">Se passar mais de 24 horas desde que você viu o problema pela primeira vez, registre um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="3f325-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3f325-117">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="3f325-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3f325-118">Aguarde pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="3f325-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="3f325-119">Se você precisar criar um novo site de equipe que não inclua um grupo do Office 365,</span><span class="sxs-lookup"><span data-stu-id="3f325-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


