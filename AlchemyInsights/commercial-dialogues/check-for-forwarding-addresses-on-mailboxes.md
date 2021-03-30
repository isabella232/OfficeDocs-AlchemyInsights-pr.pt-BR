---
title: Verifique se há endereços de encaminhamento em caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403299"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="30135-102">Verifique se há endereços de encaminhamento em caixas de correio</span><span class="sxs-lookup"><span data-stu-id="30135-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="30135-103">Às vezes, os hackers encaminham as mensagens de email dos usuários para si mesmos, então primeiro verificaremos se há endereços e regras de encaminhamento na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30135-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="30135-104">Em seguida, verificaremos os logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="30135-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="30135-105">Veja como verificar se há endereços de encaminhamento:</span><span class="sxs-lookup"><span data-stu-id="30135-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="30135-106">Selecione **Usuários**  >  **Usuários ativos**.</span><span class="sxs-lookup"><span data-stu-id="30135-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="30135-107">Selecione o usuário cuja conta foi comprometida.</span><span class="sxs-lookup"><span data-stu-id="30135-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="30135-108">No sobrevoo exibido, expanda **Configurações de Email** e clique em **Editar** para Encaminhamento **de Email.**</span><span class="sxs-lookup"><span data-stu-id="30135-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="30135-109">Remova os endereços de encaminhamento que você não reconhece.</span><span class="sxs-lookup"><span data-stu-id="30135-109">Remove any forwarding addresses you don't recognize.</span></span>