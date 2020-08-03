---
title: Pausando as atualizações agendadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530582"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="e9698-102">Pausando as atualizações agendadas</span><span class="sxs-lookup"><span data-stu-id="e9698-102">Pausing scheduled updates</span></span>

<span data-ttu-id="e9698-103">Quando um comando de pausa é emitido, os dispositivos não processam o comando até a próxima vez que eles entrarem no Intune.</span><span class="sxs-lookup"><span data-stu-id="e9698-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="e9698-104">Por causa disso, os dispositivos podem ter:</span><span class="sxs-lookup"><span data-stu-id="e9698-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="e9698-105">As atualizações agendadas foram instaladas antes do check-in.</span><span class="sxs-lookup"><span data-stu-id="e9698-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="e9698-106">Sido desligado ao emitir o comando pausar.</span><span class="sxs-lookup"><span data-stu-id="e9698-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="e9698-107">Nesse caso, quando os dispositivos estiverem ligados, eles poderão ter baixado e instalado as atualizações agendadas antes de check-in.</span><span class="sxs-lookup"><span data-stu-id="e9698-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>