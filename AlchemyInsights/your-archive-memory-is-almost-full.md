---
title: Sua caixa de correio de arquivo morto está quase cheia
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950501"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="479db-102">Sua caixa de correio de arquivo morto está quase cheia</span><span class="sxs-lookup"><span data-stu-id="479db-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="479db-103">Se o usuário receber o aviso; **Sua caixa de correio de arquivo** morto está quase cheia ou você precisa aumentar o tamanho da caixa de correio de arquivo morto, aqui estão algumas dicas:</span><span class="sxs-lookup"><span data-stu-id="479db-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="479db-104">Se o usuário tiver uma licença do Plano 1 do Exchange Online, atualize para o **Plano 2** do Exchange Online para aumentar o tamanho de 50 GB para 100 GB.</span><span class="sxs-lookup"><span data-stu-id="479db-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="479db-105">Se o usuário já tiver atribuído um dos seguintes: Plano **2** do Exchange Online ou Um Plano 1 do Exchange Online com um complemento de Arquivamento do Exchange Online, use as etapas abaixo para habilitar o arquivamento de Expansão Automática:.</span><span class="sxs-lookup"><span data-stu-id="479db-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="479db-106">[Conecte-se ao Powershell do Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="479db-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="479db-107">Execute o seguinte commandlet para o usuário:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="479db-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="479db-108">Execute o seguinte commandlet para confirmar se ele está habilitado para o usuário:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="479db-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="479db-109">Para obter mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="479db-109">For more information see:</span></span>

- [<span data-ttu-id="479db-110"> Habilitar arquivamento ilimitado - Ajuda para Administradores - Microsoft 365 Compliance | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="479db-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="479db-111">Limites do Exchange Online - Descrições de | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="479db-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="479db-112">Atualizar para um plano de negócios | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="479db-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

