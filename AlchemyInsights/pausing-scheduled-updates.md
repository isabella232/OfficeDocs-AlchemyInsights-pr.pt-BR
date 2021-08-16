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
ms.openlocfilehash: 7ea6c56de00a52080c4a8b47eb5eeee37838420a9e979878c10aeb12885a8b99
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010460"
---
# <a name="pausing-scheduled-updates"></a>Pausando as atualizações agendadas

Quando um comando de pausa é emitido, os dispositivos não processam o comando até a próxima vez que fazem check-in no Intune. Por isso, seus dispositivos podem ter:

- As atualizações agendadas foram instaladas antes do check-in.
- Foi desligado quando você emitiu o comando pause. Nesse caso, quando os dispositivos estavam ligados, eles podem ter baixado e instalado as atualizações agendadas antes do check-in.