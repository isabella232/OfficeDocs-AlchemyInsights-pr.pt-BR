---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750652"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8ceeb-102">Restringir o acesso no SharePoint ou no OneDrive</span><span class="sxs-lookup"><span data-stu-id="8ceeb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8ceeb-103">Há várias maneiras de restringir o acesso aos serviços do SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="8ceeb-104">Esses vários métodos de restrição de acesso são descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="8ceeb-105">**Restrição de permissão**</span><span class="sxs-lookup"><span data-stu-id="8ceeb-105">**Permission Restriction**</span></span>

<span data-ttu-id="8ceeb-106">No SharePoint Online e no OneDrive for Business, restringe o acesso a itens como sites, arquivos e pastas concedendo acesso apenas aos grupos/pessoas que devem ter acesso.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="8ceeb-107">Personalizar permissões para uma lista ou biblioteca do SharePoint</span><span class="sxs-lookup"><span data-stu-id="8ceeb-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="8ceeb-108">Personalizar as permissões de site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="8ceeb-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="8ceeb-109">Alterar as permissões em uma subpasta</span><span class="sxs-lookup"><span data-stu-id="8ceeb-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="8ceeb-110">Controlar o acesso de dispositivos não gerenciados</span><span class="sxs-lookup"><span data-stu-id="8ceeb-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="8ceeb-111">Como um administrador do SharePoint ou global no Office 365, você pode bloquear ou limitar o acesso ao conteúdo do SharePoint e do OneDrive de dispositivos não gerenciados (aqueles não associados ao AD híbrido ou em conformidade no Intune).</span><span class="sxs-lookup"><span data-stu-id="8ceeb-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="8ceeb-112">**Restrição de local de rede**</span><span class="sxs-lookup"><span data-stu-id="8ceeb-112">**Network Location Restriction**</span></span>

<span data-ttu-id="8ceeb-113">Como um administrador de ti, você pode controlar o acesso aos recursos do SharePoint e do OneDrive com base em locais de rede definidos nos quais confia.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="8ceeb-114">Isso também é conhecido como política baseada em local.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-114">This is also known as location-based policy.</span></span> <span data-ttu-id="8ceeb-115">Para obter mais informações, consulte [controlar o acesso aos dados do SharePoint Online e do onedrive com base no local da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="8ceeb-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="8ceeb-116">**Restrição de bloqueio de site**</span><span class="sxs-lookup"><span data-stu-id="8ceeb-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="8ceeb-117">No SharePoint Online, você pode bloquear um conjunto de sites, portanto ninguém tem acesso.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="8ceeb-118">Isso é definido por meio do PowerShell e do [Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a propriedade [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="8ceeb-119">**Impedir que os usuários criem sites ou subsites**</span><span class="sxs-lookup"><span data-stu-id="8ceeb-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="8ceeb-120">Como administrador do SharePoint ou administrador global do Office 365, você pode permitir que os usuários criem e administrem seus próprios sites do SharePoint, determine o tipo de sites que eles podem criar e especifique o local dos sites.</span><span class="sxs-lookup"><span data-stu-id="8ceeb-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="8ceeb-121">Para obter mais informações, consulte [gerenciar a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="8ceeb-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

