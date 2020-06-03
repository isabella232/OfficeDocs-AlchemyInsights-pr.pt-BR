---
title: Não é possível excluir itens no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511964"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="04cc2-102">Não é possível excluir itens</span><span class="sxs-lookup"><span data-stu-id="04cc2-102">Unable to delete items</span></span>

<span data-ttu-id="04cc2-103">As políticas de retenção podem causar isso, você precisa desabilitar ou excluir o respectivo bloqueio que está causando esse problema.</span><span class="sxs-lookup"><span data-stu-id="04cc2-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="04cc2-104">Depois que uma política de retenção ou uma retenção for removida, pode levar até 24 horas para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="04cc2-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="04cc2-105">Certifique-se de que não haja uma configuração de [política de retenção](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) no item.</span><span class="sxs-lookup"><span data-stu-id="04cc2-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="04cc2-106">O site pode ter excedido o limite de armazenamento, aumentar a [cota do site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e excluir o item.</span><span class="sxs-lookup"><span data-stu-id="04cc2-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="04cc2-107">Verifique se o item não está [com check-out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="04cc2-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="04cc2-108">Por fim, os administradores podem usar o PnP ( [padrões e práticas do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) ) que contém uma biblioteca de comandos do PowerShell que permitem executar ações complexas de gerenciamento, como forçar exclusão de itens do Stubborn.</span><span class="sxs-lookup"><span data-stu-id="04cc2-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="04cc2-109">Remover arquivo PNP</span><span class="sxs-lookup"><span data-stu-id="04cc2-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="04cc2-110">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="04cc2-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="04cc2-111">Remover item de lista PNP</span><span class="sxs-lookup"><span data-stu-id="04cc2-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="04cc2-112">Remover lista PNP</span><span class="sxs-lookup"><span data-stu-id="04cc2-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="04cc2-113">Remover campo PNP (coluna)</span><span class="sxs-lookup"><span data-stu-id="04cc2-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)