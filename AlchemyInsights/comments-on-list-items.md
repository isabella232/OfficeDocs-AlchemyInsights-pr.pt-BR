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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724142"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="878d0-102">Comentários sobre itens de lista</span><span class="sxs-lookup"><span data-stu-id="878d0-102">Comments on List items</span></span>

<span data-ttu-id="878d0-103">Os usuários podem exibir todos os comentários em um item de lista e filtrar entre modos de exibição que mostram comentários ou atividades relacionadas a um item.</span><span class="sxs-lookup"><span data-stu-id="878d0-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="878d0-104">Os usuários precisam observar o seguinte antes de poderem adicionar e excluir comentários:</span><span class="sxs-lookup"><span data-stu-id="878d0-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="878d0-105">Os comentários seguem as configurações de permissão inerentes no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="878d0-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="878d0-106">Listas clássicas que ainda não foram criadas para exibição em interfaces de usuário modernas, como listas de tarefas, não terão este recurso de comentários.</span><span class="sxs-lookup"><span data-stu-id="878d0-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="878d0-107">O comentário em listas no Microsoft Teams não está disponível nesta versão.</span><span class="sxs-lookup"><span data-stu-id="878d0-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="878d0-108">Os comentários não são indexados pela pesquisa.</span><span class="sxs-lookup"><span data-stu-id="878d0-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="878d0-109">Os administradores podem desabilitar esse recurso no nível da organização alterando o parâmetro **CommentsOnListItemsDisabled** no cmdlet do PowerShell **set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="878d0-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="878d0-110">No momento, não é possível desabilitar o comentário no nível do site ou da lista.</span><span class="sxs-lookup"><span data-stu-id="878d0-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="878d0-111">Esperamos ter esses controles em uma atualização posterior, provavelmente no primeiro trimestre de 2021.</span><span class="sxs-lookup"><span data-stu-id="878d0-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
