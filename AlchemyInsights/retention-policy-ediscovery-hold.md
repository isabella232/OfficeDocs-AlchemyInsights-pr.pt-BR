---
title: 2609-retenção-ou-descoberta eletrônica
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994042"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="d8a86-102">Não é possível excluir itens no SharePoint Online ou no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="d8a86-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="d8a86-103">Você ou seus usuários podem não conseguir excluir itens no SharePoint Online ou no OneDrive for Business porque uma política de retenção, um rótulo de retenção ou um bloqueio de descoberta eletrônica é aplicado a um SharePoint do site do OneDrive ou a um item específico.</span><span class="sxs-lookup"><span data-stu-id="d8a86-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="d8a86-104">Isso inclui ser incapaz de excluir um documento, uma versão do documento, uma pasta, uma biblioteca de documentos, uma lista, um aplicativo, um site ou um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="d8a86-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="d8a86-105">Veja a seguir alguns exemplos de mensagens de erro que você pode receber se tentar excluir um item que está sendo mantido:</span><span class="sxs-lookup"><span data-stu-id="d8a86-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="d8a86-106">"Este site não pode ser excluído porque está incluído em uma política de retenção ou bloqueio de descoberta eletrônica"</span><span class="sxs-lookup"><span data-stu-id="d8a86-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d8a86-107">"Este site tem um conjunto de políticas de conformidade para bloquear a exclusão"</span><span class="sxs-lookup"><span data-stu-id="d8a86-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="d8a86-108">"Uma política de conformidade está bloqueando atualmente esta exclusão de site"</span><span class="sxs-lookup"><span data-stu-id="d8a86-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="d8a86-109">"Este conjunto de sites não pode ser excluído porque contém sites incluídos em uma política de retenção ou bloqueio de descoberta eletrônica"</span><span class="sxs-lookup"><span data-stu-id="d8a86-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d8a86-110">"É necessário excluir todos os itens dessa pasta antes de excluir a pasta"</span><span class="sxs-lookup"><span data-stu-id="d8a86-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="d8a86-111">"Não é possível excluir as versões desse item porque elas estão em retenção ou política de retenção"</span><span class="sxs-lookup"><span data-stu-id="d8a86-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="d8a86-112">"O item não pode ser excluído enquanto estiver em espera"</span><span class="sxs-lookup"><span data-stu-id="d8a86-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="d8a86-113">"O rótulo aplicado a este item impede que ele seja editado ou excluído"</span><span class="sxs-lookup"><span data-stu-id="d8a86-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="d8a86-114">"A lista não pode ser excluída enquanto estiver em uma política de retenção ou bloqueio"</span><span class="sxs-lookup"><span data-stu-id="d8a86-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="d8a86-115">"A lista não pode ser excluída se estiver bloqueada ou se uma política de retenção for aplicada a ela"</span><span class="sxs-lookup"><span data-stu-id="d8a86-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="d8a86-116">Para excluir itens em um desses cenários, a política de retenção, o rótulo de retenção ou a descoberta eletrônica deve ser removido (ou um site deve ser excluído de uma política de retenção).</span><span class="sxs-lookup"><span data-stu-id="d8a86-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="d8a86-117">Você precisa desabilitar ou excluir o respectivo bloqueio que está causando esse problema.</span><span class="sxs-lookup"><span data-stu-id="d8a86-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="d8a86-118">Depois que uma política de retenção ou uma retenção for removida, pode levar até 24 horas para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="d8a86-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="d8a86-119">Para obter informações sobre os diferentes recursos de retenção e retenção que podem ser aplicados a sites do SharePoint e contas do OneDrive, consulte um dos tópicos a seguir.</span><span class="sxs-lookup"><span data-stu-id="d8a86-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="d8a86-120">Visão geral de políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="d8a86-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="d8a86-121">Visão geral de rótulos de retenção</span><span class="sxs-lookup"><span data-stu-id="d8a86-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="d8a86-122">Gerenciar isenções na descoberta eletrônica avançada</span><span class="sxs-lookup"><span data-stu-id="d8a86-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="d8a86-123">bloqueios de descoberta eletrônica</span><span class="sxs-lookup"><span data-stu-id="d8a86-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="d8a86-124">Políticas de fechamento e exclusão de site herdado</span><span class="sxs-lookup"><span data-stu-id="d8a86-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
