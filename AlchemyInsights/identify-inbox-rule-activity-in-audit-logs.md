---
title: Identificar a atividade da regra de caixa de entrada nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755026"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="90de3-102">Identificar a atividade da regra de caixa de entrada nos logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="90de3-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="90de3-103">Você pode usar a pesquisa de log de auditoria no centro de conformidade de & de segurança para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).</span><span class="sxs-lookup"><span data-stu-id="90de3-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="90de3-104">Faça logon no [centro de conformidade & segurança do Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="90de3-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="90de3-105">Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="90de3-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="90de3-106">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="90de3-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="90de3-107">Em **atividades de caixa de correio do Exchange**, verifique se o campo **atividades** está definido como **New-InboxRule criar/modificar/habilitar/desabilitar regra de caixa de entrada**.</span><span class="sxs-lookup"><span data-stu-id="90de3-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="90de3-108">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="90de3-108">Click **Search**.</span></span>

<span data-ttu-id="90de3-109">Nos resultados, selecione um registro de auditoria.</span><span class="sxs-lookup"><span data-stu-id="90de3-109">In the results, select an audit record.</span></span> <span data-ttu-id="90de3-110">No submenu detalhes, clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="90de3-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="90de3-111">As informações sobre as configurações da regra de caixa de entrada são exibidas no campo **parâmetros** .</span><span class="sxs-lookup"><span data-stu-id="90de3-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="90de3-112">Para obter mais informações, consulte [determinando se um usuário criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="90de3-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
