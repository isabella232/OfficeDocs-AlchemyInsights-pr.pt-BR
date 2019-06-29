---
title: Identificar o encaminhamento de emails externos em caixas de correio em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383085"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="944c4-102">Identificar quando o encaminhamento de email externo é configurado em caixas de correio</span><span class="sxs-lookup"><span data-stu-id="944c4-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="944c4-103">Quando um usuário configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="944c4-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="944c4-104">Você pode ver a atividade usando a pesquisa de log de auditoria no centro de conformidade de & de segurança.</span><span class="sxs-lookup"><span data-stu-id="944c4-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="944c4-105">Faça logon no [centro de conformidade & segurança do Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="944c4-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="944c4-106">Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="944c4-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="944c4-107">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="944c4-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="944c4-108">Não é necessário especificar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="944c4-108">You don't need to specify a username.</span></span> <span data-ttu-id="944c4-109">Verifique se o campo **atividades** está definido para **Mostrar os resultados de todas as atividades**.</span><span class="sxs-lookup"><span data-stu-id="944c4-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="944c4-110">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="944c4-110">Click **Search**.</span></span>

<span data-ttu-id="944c4-111">Nos resultados, clique em **filtrar resultados** e digite **Set-Mailbox** na caixa filtro de atividade.</span><span class="sxs-lookup"><span data-stu-id="944c4-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="944c4-112">Selecione um registro de auditoria nos resultados.</span><span class="sxs-lookup"><span data-stu-id="944c4-112">Select an audit record in the results.</span></span> <span data-ttu-id="944c4-113">No submenu **detalhes** , clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="944c4-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="944c4-114">Você precisa examinar os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.</span><span class="sxs-lookup"><span data-stu-id="944c4-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="944c4-115">**ObjectID**: o valor do alias da caixa de correio que foi modificado.</span><span class="sxs-lookup"><span data-stu-id="944c4-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="944c4-116">**Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.</span><span class="sxs-lookup"><span data-stu-id="944c4-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="944c4-117">**Userid**: o usuário que configurou o encaminhamento de emails na caixa de correio no campo **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="944c4-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="944c4-118">Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="944c4-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
