---
title: Identificar a atividade da regra de caixa de entrada nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779039"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="85a94-102">Identificar a atividade da regra de caixa de entrada nos logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="85a94-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="85a94-103">Você pode usar a pesquisa de log de auditoria no centro de conformidade & segurança da Microsoft 365 para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).</span><span class="sxs-lookup"><span data-stu-id="85a94-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="85a94-104">Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="85a94-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="85a94-105">Vá para a **Search**  >  página**pesquisa de log de auditoria** de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="85a94-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="85a94-106">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="85a94-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="85a94-107">Em **atividades de caixa de correio do Exchange**, verifique se o campo **atividades** está definido como **New-InboxRule criar/modificar/habilitar/desabilitar regra de caixa de entrada**.</span><span class="sxs-lookup"><span data-stu-id="85a94-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="85a94-108">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="85a94-108">Click **Search**.</span></span>

<span data-ttu-id="85a94-109">Nos resultados, selecione um registro de auditoria.</span><span class="sxs-lookup"><span data-stu-id="85a94-109">In the results, select an audit record.</span></span> <span data-ttu-id="85a94-110">No submenu detalhes, clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="85a94-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="85a94-111">As informações sobre as configurações da regra de caixa de entrada são exibidas no campo **parâmetros** .</span><span class="sxs-lookup"><span data-stu-id="85a94-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="85a94-112">Para obter mais informações, consulte [determinando se um usuário criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="85a94-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
