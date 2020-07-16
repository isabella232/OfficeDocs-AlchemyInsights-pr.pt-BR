---
title: Problemas com integração de computadores
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45138994"
---
# <a name="issues-with-onboarding-machines"></a>Problemas com integração de computadores

Você pode ter problemas integrando os computadores com o serviço MDATP. Se você puder acessar o computador do usuário final, siga estas etapas:

1. Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://aka.ms/mdatpanalyzer).
2. Extraia e execute MDATPAnalyzer.cmd.
3. Localize o log de diagnóstico na pasta chamada MDATPClientAnalyzerResult, a mesma pasta em que a ferramenta Analisador é baixada.
4. Examine o arquivo de log, MDATPClientAnalyzer.txt para encontrar problemas de conectividade ou configurações de proxy da internet.