---
title: Permissões de calendário
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819896"
---
# <a name="calendar-permissions"></a><span data-ttu-id="8f5d7-102">Permissões de calendário</span><span class="sxs-lookup"><span data-stu-id="8f5d7-102">Calendar Permissions</span></span>

<span data-ttu-id="8f5d7-103">Os usuários podem alterar suas próprias Permissões de Calendário com o Outlook na Web ou outros clientes, mas, como administrador, talvez seja necessário investigar também.</span><span class="sxs-lookup"><span data-stu-id="8f5d7-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="8f5d7-104">Com o cmdlet do Exchange PowerShell, você mostrará a permissão no calendário de um usuário:</span><span class="sxs-lookup"><span data-stu-id="8f5d7-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="8f5d7-105">Para ver mais informações, consulte o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8f5d7-105">To see more information see the following:</span></span>

- [<span data-ttu-id="8f5d7-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8f5d7-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="8f5d7-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8f5d7-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="8f5d7-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8f5d7-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="8f5d7-109">Permissões de calendário são usadas no compartilhamento de calendários, para ver mais informações sobre o compartilhamento de um calendário do Outlook, consulte estes artigos:</span><span class="sxs-lookup"><span data-stu-id="8f5d7-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="8f5d7-110">Compartilhar um calendário do Outlook com outras pessoas </span><span class="sxs-lookup"><span data-stu-id="8f5d7-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="8f5d7-111">Compartilhar seu calendário no Outlook na Web para empresas</span><span class="sxs-lookup"><span data-stu-id="8f5d7-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="8f5d7-112">Para solucionar problemas de Permissão de Calendário, você pode usar a [ferramenta Assistente de Suporte e](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) Recuperação.</span><span class="sxs-lookup"><span data-stu-id="8f5d7-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>