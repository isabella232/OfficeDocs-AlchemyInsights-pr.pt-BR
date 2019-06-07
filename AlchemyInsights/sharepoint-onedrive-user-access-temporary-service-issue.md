---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719505"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="0fd70-102">SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários</span><span class="sxs-lookup"><span data-stu-id="0fd70-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="0fd70-103">Se um site do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="0fd70-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="0fd70-104">[Verifique o painel de integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="0fd70-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="0fd70-105">Adicionar e licenciar o usuário</span><span class="sxs-lookup"><span data-stu-id="0fd70-105">Add and license the user</span></span>

<span data-ttu-id="0fd70-106">Certifique-se de [atribuir licenças aos usuários no Office 365 para empresas](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="0fd70-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="0fd70-107">Atribuir permissões</span><span class="sxs-lookup"><span data-stu-id="0fd70-107">Assign Permissions</span></span>

<span data-ttu-id="0fd70-108">Se o usuário tiver recebido uma licença do SharePoint e ainda estiver recebendo uma mensagem de acesso negado, verifique se ele tem o [nível de permissão apropriado](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) atribuído.</span><span class="sxs-lookup"><span data-stu-id="0fd70-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="0fd70-109">Considere usar o recurso de solicitação de acesso</span><span class="sxs-lookup"><span data-stu-id="0fd70-109">Consider using the access request feature</span></span>

<span data-ttu-id="0fd70-110">O [recurso de solicitação de acesso](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite que as pessoas solicitem acesso ao conteúdo que eles não têm permissão para ver no momento.</span><span class="sxs-lookup"><span data-stu-id="0fd70-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="0fd70-111">Permitir que o script personalizado possa causar problemas de acesso negado</span><span class="sxs-lookup"><span data-stu-id="0fd70-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="0fd70-112">Há determinados cenários em que o recurso *permitir script personalizado* pode estar apresentando um acesso negado.</span><span class="sxs-lookup"><span data-stu-id="0fd70-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="0fd70-113">Para obter uma lista dos recursos afetados, considerações sobre segurança e a capacidade de desabilitar o recurso.</span><span class="sxs-lookup"><span data-stu-id="0fd70-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="0fd70-114">Visite [permitir ou impedir o script personalizado](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="0fd70-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>
