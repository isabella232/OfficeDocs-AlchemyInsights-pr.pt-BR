---
title: Encontrar eventos executados em regras de caixa de entrada
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464348"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="31a29-102">Encontrar eventos executados em regras de caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="31a29-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="31a29-103">Quando as regras de caixa de entrada são criadas, alteradas ou excluídas, os eventos são gravados no log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="31a29-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="31a29-104">Veja como revisá-los:</span><span class="sxs-lookup"><span data-stu-id="31a29-104">Here's how to review them:</span></span>

1. <span data-ttu-id="31a29-105">Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="31a29-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="31a29-106">Selecione Pesquisar > pesquisa de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="31a29-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="31a29-107">Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora.</span><span class="sxs-lookup"><span data-stu-id="31a29-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="31a29-108">Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="31a29-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="31a29-109">Selecione o campo Atividades e encontre atividades de caixa de correio do Exchange e selecione criar New-InboxRule regra de caixa de entrada do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="31a29-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="31a29-110">Quando terminar, clique fora do painel para minimizar o painel Atividades.</span><span class="sxs-lookup"><span data-stu-id="31a29-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="31a29-111">Especifique o intervalo de datas e, em seguida, no campo Usuários, selecione o nome de usuário do usuário que você deseja investigar.</span><span class="sxs-lookup"><span data-stu-id="31a29-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="31a29-112">Você pode selecionar mais de um usuário por vez.</span><span class="sxs-lookup"><span data-stu-id="31a29-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="31a29-113">Selecione Pesquisar.</span><span class="sxs-lookup"><span data-stu-id="31a29-113">Select Search.</span></span> <span data-ttu-id="31a29-114">As atividades aparecem em Resultados.</span><span class="sxs-lookup"><span data-stu-id="31a29-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="31a29-115">Para exibir detalhes, selecione uma atividade e selecione Mais Informações.</span><span class="sxs-lookup"><span data-stu-id="31a29-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="31a29-116">Na seção Parâmetros, você pode ver o nome da regra, das condições definidas e das ações que a regra tomará.</span><span class="sxs-lookup"><span data-stu-id="31a29-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="31a29-117">Para saber mais, confira Pesquisar o log de auditoria do Office 365 para solucionar problemas de cenários comuns.</span><span class="sxs-lookup"><span data-stu-id="31a29-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>