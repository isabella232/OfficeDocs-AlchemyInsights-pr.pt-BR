---
title: Eventos de calendário ausentes ou desatualizados
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819976"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="d124f-102">Eventos de Calendário ausentes ou desatualizados</span><span class="sxs-lookup"><span data-stu-id="d124f-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="d124f-103">Se os itens do calendário estiverem ausentes ou desatualizados, comece por analisando a contagem dos itens nas propriedades da pasta Calendário no Outlook:</span><span class="sxs-lookup"><span data-stu-id="d124f-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="d124f-104">Clique com o botão direito do mouse na pasta **Calendário** do usuário afetado e, em seguida, selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="d124f-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="d124f-105">Selecione a guia **Sincronização**.</span><span class="sxs-lookup"><span data-stu-id="d124f-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="d124f-106">Se a contagem de itens não for a mesma entre a Pasta do Servidor e a Pasta Offline:</span><span class="sxs-lookup"><span data-stu-id="d124f-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="d124f-107">Realce a pasta **Calendário**.</span><span class="sxs-lookup"><span data-stu-id="d124f-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="d124f-108">Vá para a guia **Enviar**/**Receber** e selecione **Atualizar Pasta**.</span><span class="sxs-lookup"><span data-stu-id="d124f-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="d124f-109">Se o calendário ainda estiver desatualizado, ou se os eventos estiverem ausentes, baixe a Ferramenta de Verificação de Calendário para Outlook no [Centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=28786).</span><span class="sxs-lookup"><span data-stu-id="d124f-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="d124f-110">Determine se há mais de 5.000 itens na pasta do calendário, pois isso poderá causar sintomas como reuniões de calendário desatualizadas ou erros de reunião.</span><span class="sxs-lookup"><span data-stu-id="d124f-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="d124f-111">Para saber mais, confira [Problemas de desempenho do Outlook quando há vários itens ou pastas em um arquivo .ost ou .pst em modo cache](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="d124f-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>