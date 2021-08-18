---
title: Solucionar problemas de instalação do MDATP em um Mac
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090964"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Solucionar problemas de instalação do MDATP em um Mac

Se a instalação manual falhar, a página **Resumo** do assistente de instalação mostrará o seguinte erro:

"Ocorreu um erro durante a instalação. O Instalador encontrou um erro que causou a falha da instalação. Entre em contato com o fabricante do software para assistência."

Para implantações MDM, a página também mostra uma falha de instalação genérica.

Embora não exibemos erros exatos para os usuários finais, manteremos um arquivo de log com progresso de instalação, em **/Library/Logs/Microsoft/mdatp/install.log**. Cada sessão de instalação é anexada a esse arquivo de log. Para saída somente da última sessão de instalação, use `sed` .

Para saber mais, confira [Solucionar problemas de instalação do Microsoft Defender ATP para Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
