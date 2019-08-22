---
title: Identificar endereço IP e cliente em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539017"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="97cb2-102">Identificar endereço IP e cliente em logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="97cb2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="97cb2-103">O endereço IP que corresponde a uma atividade por um usuário ou administrador do Office 365 é mostrado nos logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="97cb2-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="97cb2-104">As informações do cliente também são registradas.</span><span class="sxs-lookup"><span data-stu-id="97cb2-104">The client information is also logged.</span></span> <span data-ttu-id="97cb2-105">Aqui estão as etapas para identificar essas informações</span><span class="sxs-lookup"><span data-stu-id="97cb2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="97cb2-106">Faça logon no [centro de conformidade & segurança do Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="97cb2-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="97cb2-107">Vá para a página**pesquisa de log de auditoria** de **pesquisa** > .</span><span class="sxs-lookup"><span data-stu-id="97cb2-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="97cb2-108">Se você estiver interessado em uma atividade específica, selecione-a na lista de **atividades** .</span><span class="sxs-lookup"><span data-stu-id="97cb2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="97cb2-109">Caso contrário, todas as atividades serão retornadas para o usuário selecionado (configuração padrão).</span><span class="sxs-lookup"><span data-stu-id="97cb2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="97cb2-110">**Observação**: determinadas atividades podem não estar disponíveis no menu **atividades** ; no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** for selecionado (configuração padrão).</span><span class="sxs-lookup"><span data-stu-id="97cb2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="97cb2-111">Especifique o nome de usuário no campo **usuários** , selecione o intervalo de datas apropriado para a atividade e clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="97cb2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="97cb2-112">Nos resultados, você pode ver o endereço IP dessa atividade no painel de resultados.</span><span class="sxs-lookup"><span data-stu-id="97cb2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="97cb2-113">Selecione o registro de auditoria para ver informações detalhadas no submenu **detalhes** (por exemplo, cliente, usuário que executou a ação, etc.).</span><span class="sxs-lookup"><span data-stu-id="97cb2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="97cb2-114">Para obter mais informações, consulte [localizar o endereço IP do computador usado para acessar uma conta comprometida](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="97cb2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
