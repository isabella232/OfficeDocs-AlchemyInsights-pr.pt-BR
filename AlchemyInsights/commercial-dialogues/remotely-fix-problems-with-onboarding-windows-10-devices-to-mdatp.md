---
title: Corrigir remotamente problemas com a integração Windows 10 dispositivos para a Proteção Avançada contra Ameaças do Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034022"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Corrigir remotamente problemas com a integração Windows 10 dispositivos para a Proteção Avançada contra Ameaças do Microsoft Defender

Se você puder acessar o computador remoto, siga estas etapas:

1. Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Extraia e execute MDATPAnalyzer.cmd.
3. Localize o log de diagnóstico na pasta MDATPClientAnalyzerResult, que é a mesma pasta onde a ferramenta Analisador foi baixada.
4. Para encontrar problemas com as configurações de conectividade ou proxy da Internet, revise o arquivo de log MDATPClientAnalyzer.txt.

Para saber mais, confira [Problemas com máquinas de integração.](https://go.microsoft.com/fwlink/?linkid=2143634)
