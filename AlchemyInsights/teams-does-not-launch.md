---
title: O Teams não inicia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100209"
---
# <a name="teams-doesnt-launch"></a>O Teams não inicia

Se você tentar abrir o Microsoft Teams, mas ele nunca for iniciado, tente o seguinte:

1. Navegue até **%appdata%\Microsoft\Teams**.
1. Exclua os conteúdos da pasta.
1. Reinicie o computador e tente iniciar o Teams.

Talvez seja necessário reinstalar o Teams. Para reinstalar:

1. Desinstale o Teams usando o Painel de Controle.
1. Navegue até **%appdata%\Microsoft\Teams\Application Cache**.
1. Exclua os conteúdos da pasta.
1. Navegue até **%appdata%\Microsoft\teams\Cache**.
1. Exclua os conteúdos da pasta.
1. Reinicie o computador e baixe e instale o Teams.

Se você quiser executar um diagnóstico em seu locatário para um usuário específico que não consegue entrar, inicie uma nova pesquisa com a palavra-chave **TeamsUserUnableToSignIn** e siga os prompts.