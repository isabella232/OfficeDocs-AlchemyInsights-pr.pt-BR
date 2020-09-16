---
title: Enviar como grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740139"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="d7635-102">Enviar como grupo Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d7635-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="d7635-103">Você pode atribuir permissões de “Enviar como” para permitir que certos usuários enviem mensagens como um grupo Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d7635-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="d7635-104">Conecte-se ao Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d7635-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="d7635-105">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="d7635-105">Run the following command:</span></span>  

    <span data-ttu-id="d7635-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="d7635-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="d7635-107">Para mais informações, confira [Permitir que os membros enviem email usando “Enviar como” ou “Enviar em nome de um grupo”](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d7635-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>