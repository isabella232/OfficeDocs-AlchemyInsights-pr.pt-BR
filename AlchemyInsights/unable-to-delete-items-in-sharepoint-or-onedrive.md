---
title: Não é possível excluir itens no SharePoint ou no OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757913"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="2f8c3-102">Não é possível excluir itens</span><span class="sxs-lookup"><span data-stu-id="2f8c3-102">Unable to delete items</span></span>

<span data-ttu-id="2f8c3-103">Você está tendo problemas para excluir itens?</span><span class="sxs-lookup"><span data-stu-id="2f8c3-103">Having issues deleting items?</span></span>

- <span data-ttu-id="2f8c3-104">Verifique sempre se você tem as [permissões apropriadas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) para excluir o item ou se um [administrador de conjunto de sites](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) tentou remover o item.</span><span class="sxs-lookup"><span data-stu-id="2f8c3-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="2f8c3-105">Certifique-se de que não haja uma configuração de [política de retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no item.</span><span class="sxs-lookup"><span data-stu-id="2f8c3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="2f8c3-106">Verifique se o item não está [com check-out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="2f8c3-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="2f8c3-107">Por fim, os administradores podem usar o PnP ( [padrões e práticas do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) ) que contém uma biblioteca de comandos do PowerShell que permitem executar ações complexas de gerenciamento, como forçar exclusão de itens do Stubborn.</span><span class="sxs-lookup"><span data-stu-id="2f8c3-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="2f8c3-108">Remover arquivo PNP</span><span class="sxs-lookup"><span data-stu-id="2f8c3-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="2f8c3-109">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="2f8c3-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="2f8c3-110">Remover item de lista PNP</span><span class="sxs-lookup"><span data-stu-id="2f8c3-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="2f8c3-111">Remover lista PNP</span><span class="sxs-lookup"><span data-stu-id="2f8c3-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="2f8c3-112">Remover campo PNP (coluna)</span><span class="sxs-lookup"><span data-stu-id="2f8c3-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)