---
title: Descubra quem configurar o encaminhamento em uma caixa de correio e como
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464312"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="25b56-102">Descubra quem configurar o encaminhamento em uma caixa de correio e como</span><span class="sxs-lookup"><span data-stu-id="25b56-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="25b56-103">Se o encaminhamento externo foi definido em uma caixa de correio, a atividade é auditada como parte do cmdlet Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="25b56-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="25b56-104">Veja como encontrar a atividade no log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="25b56-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="25b56-105">Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="25b56-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="25b56-106">Selecione **Pesquisa de** log de auditoria de >  **pesquisa**.</span><span class="sxs-lookup"><span data-stu-id="25b56-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="25b56-107">Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora.</span><span class="sxs-lookup"><span data-stu-id="25b56-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="25b56-108">Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="25b56-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="25b56-109">Certifique-se de **que o** campo Atividades está definido como Mostrar resultados para todas **as atividades** (o padrão).</span><span class="sxs-lookup"><span data-stu-id="25b56-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="25b56-110">Especifique o intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="25b56-110">Specify the date range.</span></span> <span data-ttu-id="25b56-111">Não é necessário especificar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="25b56-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="25b56-112">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="25b56-112">Select **Search**.</span></span> <span data-ttu-id="25b56-113">As atividades aparecem em **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="25b56-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="25b56-114">Selecione **Resultados do Filtro** e insira **Set-mailbox** no campo **Filtro** atividade.</span><span class="sxs-lookup"><span data-stu-id="25b56-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="25b56-115">Isso retorna todas **as atividades Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="25b56-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="25b56-116">Para exibir os detalhes, selecione uma atividade e selecione **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="25b56-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="25b56-117">Em **Parâmetros,** você pode ver o endereço de email de encaminhamento que foi definido na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="25b56-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="25b56-118">O **UserID** representa o usuário que configura o encaminhamento externo na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="25b56-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="25b56-119">Para saber mais, confira Pesquisar o log de auditoria do [Office 365 para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="25b56-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>