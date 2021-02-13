---
title: Bloquear assinaturas de email feitas pelo usuário
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232667"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="94e07-102">Bloquear assinaturas de email feitas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="94e07-102">Block user-made email signatures</span></span>

<span data-ttu-id="94e07-103">A solução a seguir só se aplica a assinaturas de email criadas no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="94e07-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="94e07-104">Você só pode bloquear assinaturas no aplicativo do Outlook se tiver um Exchange Server local.</span><span class="sxs-lookup"><span data-stu-id="94e07-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="94e07-105">In the admin center, choose **Admin centers**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="94e07-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="94e07-106">Clique **em permissões das** políticas do Outlook Web  >  **App.**</span><span class="sxs-lookup"><span data-stu-id="94e07-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="94e07-107">Selecione a política e clique no ícone de lápis para editá-la.</span><span class="sxs-lookup"><span data-stu-id="94e07-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="94e07-108">Clique **em recursos** Mais  >  **opções.**</span><span class="sxs-lookup"><span data-stu-id="94e07-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="94e07-109">Em **Experiência do Usuário,** des marque a **caixa de** seleção Assinatura de email e clique em **Salvar.**</span><span class="sxs-lookup"><span data-stu-id="94e07-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="94e07-110">**Importante:** Se uma assinatura foi adicionada antes de limpar essa caixa de seleção, o usuário ainda poderá usá-la.</span><span class="sxs-lookup"><span data-stu-id="94e07-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="94e07-111">Peça para eles removê-lo.</span><span class="sxs-lookup"><span data-stu-id="94e07-111">Ask them to remove it.</span></span>
