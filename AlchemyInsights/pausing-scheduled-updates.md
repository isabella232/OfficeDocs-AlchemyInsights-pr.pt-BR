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
# <a name="pausing-scheduled-updates"></a>Pausando as atualizações agendadas

Quando um comando de pausa é emitido, os dispositivos não processam o comando até a próxima vez que eles entrarem no Intune. Por causa disso, os dispositivos podem ter:

- As atualizações agendadas foram instaladas antes do check-in.
- Sido desligado ao emitir o comando pausar. Nesse caso, quando os dispositivos estiverem ligados, eles poderão ter baixado e instalado as atualizações agendadas antes de check-in.