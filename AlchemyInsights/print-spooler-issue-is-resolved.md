---
title: O problema do spooler de impressão está resolvido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801829"
---
# <a name="print-spooler-issue-is-resolved"></a>O problema do spooler de impressão está resolvido

Se o seu dispositivo foi atualizado com o Windows 10  **OS Build 19041.329**, você pode ter observado um problema onde algumas impressoras não estão conseguindo imprimir. O spooler de impressão pode exibir um erro ou fechar inesperadamente ao tentar imprimir e não há qualquer saída a partir da impressora afetada. Este problema está resolvido na versão **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigação em curso**

O arquivo do Serviço de Subsistema da Autoridade Local de Segurança (LSASS) (**Isass.exe**) pode falhar em alguns dispositivos e exibir a mensagem de erro, "Um processo crítico do sistema, C:\WINDOWS\system32\Isass.exe, falhou com o código de estatus c0000008. O computador precisa ser reiniciado agora".  **A Microsoft está trabalhando na solução e vai fornecer uma atualização no próximo lançamento.**

Para obter mais informações, verifique os problemas conhecidos do [Windows 10 Versão 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).