---
title: Comentários sobre itens de lista
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947472"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="126ff-102">Comentários sobre itens de lista</span><span class="sxs-lookup"><span data-stu-id="126ff-102">Comments on List items</span></span>

<span data-ttu-id="126ff-103">Em breve, os usuários poderão adicionar e excluir comentários em itens de lista.</span><span class="sxs-lookup"><span data-stu-id="126ff-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="126ff-104">Os usuários podem exibir todos os comentários em um item de lista e filtrar entre modos de exibição que mostram comentários ou atividades relacionadas a um item.</span><span class="sxs-lookup"><span data-stu-id="126ff-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="126ff-105">**Tempo** :</span><span class="sxs-lookup"><span data-stu-id="126ff-105">**Timing** :</span></span>

<span data-ttu-id="126ff-106">**Lançamento direcionado** : distribuição gradual em meados de outubro e esperado para conclusão em meados de novembro</span><span class="sxs-lookup"><span data-stu-id="126ff-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="126ff-107">**Versão padrão** : distribuição gradual em meados de novembro e espera-se que seja concluída pelo início de dezembro</span><span class="sxs-lookup"><span data-stu-id="126ff-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="126ff-108">**Distribuição** : lançamento direcionado para toda a organização</span><span class="sxs-lookup"><span data-stu-id="126ff-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="126ff-109">Os usuários precisam observar o seguinte antes de poderem adicionar e excluir comentários:</span><span class="sxs-lookup"><span data-stu-id="126ff-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="126ff-110">Os comentários seguem as configurações de permissão inerentes no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="126ff-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="126ff-111">Listas clássicas que ainda não foram criadas para exibição em interfaces de usuário modernas, como listas de tarefas, não terão este recurso de comentários.</span><span class="sxs-lookup"><span data-stu-id="126ff-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="126ff-112">O comentário em listas no Microsoft Teams não está disponível nesta versão.</span><span class="sxs-lookup"><span data-stu-id="126ff-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="126ff-113">Os comentários não são indexados pela pesquisa.</span><span class="sxs-lookup"><span data-stu-id="126ff-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="126ff-114">Os administradores podem desabilitar esse recurso no nível da organização alterando o parâmetro **CommentsOnListItemsDisabled** no cmdlet do PowerShell **set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="126ff-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="126ff-115">No momento, não é possível desabilitar o comentário no nível do site ou da lista.</span><span class="sxs-lookup"><span data-stu-id="126ff-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="126ff-116">Esperamos ter esses controles em uma atualização posterior, provavelmente no primeiro trimestre de 2021.</span><span class="sxs-lookup"><span data-stu-id="126ff-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
