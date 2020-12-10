---
title: 'Solucionando problemas de caixa postal '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607991"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="c5768-102">Solucionando problemas de caixa postal</span><span class="sxs-lookup"><span data-stu-id="c5768-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="c5768-103">Verifique se o recurso ocupado no ocupado é intencional.</span><span class="sxs-lookup"><span data-stu-id="c5768-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="c5768-104">Se este recurso não é necessário para este usuário:</span><span class="sxs-lookup"><span data-stu-id="c5768-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="c5768-105">Vá para o centro de administração do Microsoft [Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="c5768-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="c5768-106">No trilho esquerdo, navegue pelas  >  **políticas**  >  de chamada de voz **gerencie políticas** na política de **chamada**.</span><span class="sxs-lookup"><span data-stu-id="c5768-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="c5768-107">Selecione **gerenciar usuários**.</span><span class="sxs-lookup"><span data-stu-id="c5768-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="c5768-108">Pesquise o usuário e altere a política de chamada para um que esteja **ocupado quando ocupado estiver disponível quando estiver em uma chamada** para **desativar**.</span><span class="sxs-lookup"><span data-stu-id="c5768-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="c5768-109">Clique em **Aplicar**.</span><span class="sxs-lookup"><span data-stu-id="c5768-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="c5768-110">As alterações nas políticas podem levar até 24 horas para serem replicadas.</span><span class="sxs-lookup"><span data-stu-id="c5768-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="c5768-111">Para obter mais informações sobre esse recurso, consulte: [ocupado quando ocupado está disponível durante uma chamada](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="c5768-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
