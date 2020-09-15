---
title: Problemas com integração de computadores
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676870"
---
# <a name="issues-with-onboarding-machines"></a>Problemas com integração de computadores

Você pode ter problemas integrando os computadores com o serviço MDATP. Se você puder acessar o computador do usuário final, siga estas etapas:

1. Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://aka.ms/mdatpanalyzer).
2. Extraia e execute MDATPAnalyzer.cmd.
3. Localize o log de diagnóstico na pasta chamada MDATPClientAnalyzerResult, a mesma pasta em que a ferramenta Analisador é baixada.
4. Examine o arquivo de log, MDATPClientAnalyzer.txt para encontrar problemas de conectividade ou configurações de proxy da internet.