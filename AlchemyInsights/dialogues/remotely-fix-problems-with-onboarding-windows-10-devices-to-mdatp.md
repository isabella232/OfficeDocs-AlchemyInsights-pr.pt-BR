---
title: Corrigir remotamente problemas com a integração de dispositivos Windows 10 à Proteção Avançada contra Ameaças do Microsoft Defender
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529865"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Corrigir remotamente problemas com a integração de dispositivos Windows 10 à Proteção Avançada contra Ameaças do Microsoft Defender

Se você puder acessar o computador remoto, siga estas etapas:

1. Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Extraia e execute MDATPAnalyzer.cmd.
3. Localize o log de diagnóstico na pasta MDATPClientAnalyzerResult, que é a mesma pasta onde a ferramenta Analisador foi baixada.
4. Para encontrar problemas com as configurações de conectividade ou proxy da Internet, revise o arquivo de log MDATPClientAnalyzer.txt.

Para saber mais, confira [Problemas com máquinas de integração.](https://go.microsoft.com/fwlink/?linkid=2143634)
