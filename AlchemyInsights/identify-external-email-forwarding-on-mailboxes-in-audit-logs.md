---
title: Identificar o encaminhamento de emails externos em caixas de correio em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716448"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="9851b-102">Identificar quando o encaminhamento de email externo é configurado em caixas de correio</span><span class="sxs-lookup"><span data-stu-id="9851b-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="9851b-103">Quando um usuário do Microsoft 365 configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="9851b-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="9851b-104">Você pode ver a atividade usando a pesquisa de log de auditoria no centro de conformidade de & de segurança.</span><span class="sxs-lookup"><span data-stu-id="9851b-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="9851b-105">Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9851b-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9851b-106">Vá para a página**pesquisa de log de auditoria** de **pesquisa** > .</span><span class="sxs-lookup"><span data-stu-id="9851b-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="9851b-107">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="9851b-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9851b-108">Não é necessário especificar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="9851b-108">You don't need to specify a username.</span></span> <span data-ttu-id="9851b-109">Verifique se o campo **atividades** está definido para **Mostrar os resultados de todas as atividades**.</span><span class="sxs-lookup"><span data-stu-id="9851b-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="9851b-110">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="9851b-110">Click **Search**.</span></span>

<span data-ttu-id="9851b-111">Nos resultados, clique em **filtrar resultados** e digite **Set-Mailbox** na caixa filtro de atividade.</span><span class="sxs-lookup"><span data-stu-id="9851b-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="9851b-112">Selecione um registro de auditoria nos resultados.</span><span class="sxs-lookup"><span data-stu-id="9851b-112">Select an audit record in the results.</span></span> <span data-ttu-id="9851b-113">No submenu **detalhes** , clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="9851b-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="9851b-114">Você precisa examinar os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.</span><span class="sxs-lookup"><span data-stu-id="9851b-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="9851b-115">**ObjectID**: o valor do alias da caixa de correio que foi modificado.</span><span class="sxs-lookup"><span data-stu-id="9851b-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="9851b-116">**Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.</span><span class="sxs-lookup"><span data-stu-id="9851b-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="9851b-117">**Userid**: o usuário que configurou o encaminhamento de emails na caixa de correio no campo **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="9851b-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="9851b-118">Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9851b-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
