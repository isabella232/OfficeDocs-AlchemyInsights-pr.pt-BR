---
title: 618 política de compartilhamento de calendário
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684218"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="11163-102">Erro de política ao compartilhar um calendário</span><span class="sxs-lookup"><span data-stu-id="11163-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="11163-103">Execute um dos seguintes procedimentos, conforme apropriado para sua situação:</span><span class="sxs-lookup"><span data-stu-id="11163-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="11163-104">Conecte-se ao Exchange Online usando o PowerShell remoto.</span><span class="sxs-lookup"><span data-stu-id="11163-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="11163-105">Para obter mais informações, consulte [conectar-se ao Exchange Online usando o PowerShell remoto](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="11163-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="11163-106">No servidor local, abra o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11163-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="11163-107">Determine a política de compartilhamento que é atribuída ao usuário.</span><span class="sxs-lookup"><span data-stu-id="11163-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="11163-108">Para fazer isso, execute o seguinte comando e anote a política retornada:</span><span class="sxs-lookup"><span data-stu-id="11163-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="11163-109">Atualize a política de compartilhamento para o usuário.</span><span class="sxs-lookup"><span data-stu-id="11163-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="11163-110">Para fazer isso, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="11163-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="11163-111">Abra o centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11163-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="11163-112">Clique em **organização**e, em seguida, clique duas vezes na política atribuída ao usuário em **compartilhamento individual**.</span><span class="sxs-lookup"><span data-stu-id="11163-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="11163-113">Esta é a política retornada na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="11163-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="11163-114">Na página regra de compartilhamento, selecione o nível de compartilhamento de calendário que você deseja permitir em **especifique quais informações você deseja compartilhar**; clique em **salvar**.</span><span class="sxs-lookup"><span data-stu-id="11163-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="11163-115">Para obter mais informações, consulte: ["a política não permite conceder permissões neste nível a um ou mais dos destinatários" quando o usuário tenta compartilhar o calendário](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="11163-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
