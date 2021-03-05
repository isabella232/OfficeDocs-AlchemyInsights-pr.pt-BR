---
title: Ler os logs de auditoria para eventos excluídos
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464308"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="97763-102">Ler os logs de auditoria para eventos excluídos</span><span class="sxs-lookup"><span data-stu-id="97763-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="97763-103">Veja como fazer isso:</span><span class="sxs-lookup"><span data-stu-id="97763-103">Here's how to do this:</span></span>

1. <span data-ttu-id="97763-104">Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="97763-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="97763-105">Selecione **Pesquisa de** log de auditoria de  >  [**pesquisa**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="97763-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="97763-106">Se você vir um aviso de que precisa ativar o recurso, vá em frente e a ligue agora.</span><span class="sxs-lookup"><span data-stu-id="97763-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="97763-107">Se o recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="97763-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="97763-108">Selecione **Atividades** e, em seguida, encontre atividades **de caixa de correio do Exchange.**</span><span class="sxs-lookup"><span data-stu-id="97763-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="97763-109">Selecione as **mensagens excluídas da pasta Itens Excluídos** e As mensagens **movidas para as opções de** pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="97763-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="97763-110">Quando terminar, clique fora do painel para minimizar o painel **Atividades.**</span><span class="sxs-lookup"><span data-stu-id="97763-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="97763-111">Especifique o intervalo de datas e, na caixa **Usuários,** selecione o nome de usuário do usuário que você deseja investigar.</span><span class="sxs-lookup"><span data-stu-id="97763-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="97763-112">Você pode selecionar mais de um usuário por vez.</span><span class="sxs-lookup"><span data-stu-id="97763-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="97763-113">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="97763-113">Select **Search**.</span></span> <span data-ttu-id="97763-114">As atividades aparecem em **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="97763-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="97763-115">Para exibir os detalhes, selecione uma atividade e selecione **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="97763-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="97763-116">Informações adicionais sobre o item excluído, como a linha de assunto e o local do item quando ele foi excluído, são exibidas no campo **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="97763-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="97763-117">Não é possível restaurar itens excluídos usando o recurso de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="97763-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="97763-118">Para restaurar itens excluídos, consulte [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="97763-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="97763-119">Para saber mais, confira Pesquisar o log de auditoria do [Office 365 para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="97763-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
