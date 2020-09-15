---
title: Pausando as atualizações agendadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721543"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="c5613-102">Pausando as atualizações agendadas</span><span class="sxs-lookup"><span data-stu-id="c5613-102">Pausing scheduled updates</span></span>

<span data-ttu-id="c5613-103">Quando um comando de pausa é emitido, os dispositivos não processam o comando até a próxima vez que eles entrarem no Intune.</span><span class="sxs-lookup"><span data-stu-id="c5613-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="c5613-104">Por causa disso, os dispositivos podem ter:</span><span class="sxs-lookup"><span data-stu-id="c5613-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="c5613-105">As atualizações agendadas foram instaladas antes do check-in.</span><span class="sxs-lookup"><span data-stu-id="c5613-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="c5613-106">Sido desligado ao emitir o comando pausar.</span><span class="sxs-lookup"><span data-stu-id="c5613-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="c5613-107">Nesse caso, quando os dispositivos estiverem ligados, eles poderão ter baixado e instalado as atualizações agendadas antes de check-in.</span><span class="sxs-lookup"><span data-stu-id="c5613-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>