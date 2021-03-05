---
title: Encontre o endereço IP no log de auditoria
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464349"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="f8843-102">Encontre o endereço IP no log de auditoria</span><span class="sxs-lookup"><span data-stu-id="f8843-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="f8843-103">O endereço IP que corresponde a uma atividade executada por um usuário ou administrador é mostrado nos logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f8843-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="f8843-104">As informações do cliente também são registradas.</span><span class="sxs-lookup"><span data-stu-id="f8843-104">The client information is also logged.</span></span> <span data-ttu-id="f8843-105">Veja como identificar o endereço IP:</span><span class="sxs-lookup"><span data-stu-id="f8843-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="f8843-106">Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="f8843-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f8843-107">Selecione **Pesquisa de** log de auditoria de  >  **[pesquisa](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="f8843-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f8843-108">Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora.</span><span class="sxs-lookup"><span data-stu-id="f8843-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f8843-109">Se esse recurso não estiver habilitado, os resultados da pesquisa não poderão puxar dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="f8843-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f8843-110">Se você estiver interessado em uma atividade específica, selecione-a na lista **Atividades;** caso contrário, por padrão, todas as atividades serão retornadas para o usuário selecionado.</span><span class="sxs-lookup"><span data-stu-id="f8843-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="f8843-111">Observe que determinadas atividades podem não estar disponíveis para seleção no menu **Atividades;** no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** estiver selecionado (configuração padrão).</span><span class="sxs-lookup"><span data-stu-id="f8843-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="f8843-112">Especifique o intervalo de datas e, no campo **Usuários,** selecione o nome de usuário do usuário que você deseja investigar.</span><span class="sxs-lookup"><span data-stu-id="f8843-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="f8843-113">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="f8843-113">Select **Search**.</span></span> <span data-ttu-id="f8843-114">As atividades aparecem em **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="f8843-114">The activities appear under **Results**.</span></span> <span data-ttu-id="f8843-115">Você pode ver o endereço IP de cada atividade.</span><span class="sxs-lookup"><span data-stu-id="f8843-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="f8843-116">Para exibir detalhes, selecione uma atividade e selecione **Mais Informações**.</span><span class="sxs-lookup"><span data-stu-id="f8843-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="f8843-117">Para saber mais, confira Pesquisar o log de auditoria do [Office 365 para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="f8843-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>