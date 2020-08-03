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
# <a name="pausing-scheduled-updates"></a>Pausando as atualizações agendadas

Quando um comando de pausa é emitido, os dispositivos não processam o comando até a próxima vez que eles entrarem no Intune. Por causa disso, os dispositivos podem ter:

- As atualizações agendadas foram instaladas antes do check-in.
- Sido desligado ao emitir o comando pausar. Nesse caso, quando os dispositivos estiverem ligados, eles poderão ter baixado e instalado as atualizações agendadas antes de check-in.