---
title: Solucionar problemas de mensagens de acesso negado
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503515"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="f0a6c-102">Solucionar problemas de mensagens de acesso negado no centro de administração do SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="f0a6c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="f0a6c-103">Se você estiver recebendo uma mensagem de acesso negado ao tentar navegar até um centro de administração do SharePoint/OneDrive, certifique-se de [atribuir uma licença ao usuário](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="f0a6c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="f0a6c-104">Se o usuário tiver uma licença, você também deve certificar-se de que ela é [atribuída a uma função de administrador](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) que pode acessar os centros de administração.</span><span class="sxs-lookup"><span data-stu-id="f0a6c-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="f0a6c-105">Esse problema também pode ocorrer quando um usuário é excluído e recriado com o mesmo nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="f0a6c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f0a6c-106">A nova conta é criada usando um valor diferente de PUID (ID exclusiva do Passport).</span><span class="sxs-lookup"><span data-stu-id="f0a6c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f0a6c-107">Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="f0a6c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f0a6c-108">Um segundo cenário envolve a sincronização de diretório com uma unidade organizacional (OU) do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0a6c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f0a6c-109">Se os usuários já tiverem entrado no SharePoint e forem movidos para uma OU diferente e ressincronizado com o SharePoint, poderão enfrentar esse problema.</span><span class="sxs-lookup"><span data-stu-id="f0a6c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="f0a6c-110">Para resolver esse problema, você deve restaurar o UPN original com as etapas no artigo, [restaurar um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f0a6c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="f0a6c-111">Observação: se um centro de administração do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="f0a6c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="f0a6c-112">[Verifique o painel de integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f0a6c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


