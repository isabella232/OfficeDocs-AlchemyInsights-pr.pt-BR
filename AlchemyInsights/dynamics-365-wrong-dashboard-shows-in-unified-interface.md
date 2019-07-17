---
title: Dynamics 365-apresentações de painel incorretas na interface unificada do Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35746869"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Apresentações de painel incorretas na interface unificada do Dynamics 365

Há várias razões pelas quais você pode ver um painel diferente do que você espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O usuário configurou um painel de usuário padrão 

Normalmente, você pode identificar um painel padrão do usuário é definido se o botão **definir como padrão** não for exibido na barra de comandos do painel. O painel padrão do usuário substituirá todos os outros painéis padrão, mesmo que o painel padrão do usuário não esteja no aplicativo atual.

Use a seguinte solução alternativa para remover o painel padrão.

1. Criar um novo painel pessoal.

2. Defina esse novo painel como o usuário padrão.

3. Exclua esse painel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O painel é definido no sitemap

Você pode ter definido um painel padrão da organização selecionando um painel e escolhendo ' definir como padrão ' em ' Personalizar o sistema '. Mas o painel definido no designer de sitemap prevalecerá sobre esse painel, se o usuário tiver acesso a ele.

Para que os usuários vejam o painel definido como o padrão da organização, você pode:

* Definir esse painel no sitemap

* Remover o acesso ao painel definido de sitemap para esses usuários
