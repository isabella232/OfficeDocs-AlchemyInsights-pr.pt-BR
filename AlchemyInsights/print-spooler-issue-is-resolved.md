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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911326"
---
# <a name="print-spooler-issue-is-resolved"></a>O problema do spooler de impressão está resolvido

Se o seu dispositivo foi atualizado com o Windows 10  **OS Build 19041.329**, você pode ter observado um problema onde algumas impressoras não estão conseguindo imprimir. O spooler de impressão pode exibir um erro ou fechar inesperadamente ao tentar imprimir e não há qualquer saída a partir da impressora afetada. Este problema está resolvido na versão **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigação em curso**

O arquivo do Serviço de Subsistema da Autoridade Local de Segurança (LSASS) (**Isass.exe**) pode falhar em alguns dispositivos e exibir a mensagem de erro, "Um processo crítico do sistema, C:\WINDOWS\system32\Isass.exe, falhou com o código de estatus c0000008. O computador precisa ser reiniciado agora".  **A Microsoft está trabalhando na solução e vai fornecer uma atualização no próximo lançamento.**

Para obter mais informações, verifique os problemas conhecidos do [Windows 10 Versão 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).