---
title: Impedir que mensagens se movem automaticamente para o arquivo morto
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735419"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="2a132-102">Impedir que mensagens se movem automaticamente para o arquivo morto</span><span class="sxs-lookup"><span data-stu-id="2a132-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="2a132-103">Se você estiver usando uma política de retenção, poderá alterar a idade de retenção nessa política para impedir que as mensagens sejam arquivadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2a132-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="2a132-104">Veja como:</span><span class="sxs-lookup"><span data-stu-id="2a132-104">Here's how:</span></span>

1. <span data-ttu-id="2a132-105">No Centro [de administração do Exchange,](https://go.microsoft.com/fwlink/?linkid=2059104)escolha **marcas de retenção de gerenciamento de**  >  **conformidade.**</span><span class="sxs-lookup"><span data-stu-id="2a132-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="2a132-106">Localize sua marca de retenção Mover para Arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="2a132-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="2a132-107">Na marca de retenção, altere o período de retenção (período de arquivamento) para **Nunca** para impedir que os itens são arquivados automaticamente por uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="2a132-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="2a132-108">Isso alterará a configuração de arquivo morto para todas as caixas de correio com essa marca de retenção aplicada a elas.</span><span class="sxs-lookup"><span data-stu-id="2a132-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
