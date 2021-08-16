---
title: Dynamics 365 - Painel Errado Mostra na Interface Unificada do Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101470"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Painel errado mostra na interface unificada do Dynamics 365

Há vários motivos pelos quais você pode ver um painel diferente do esperado:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O usuário definiu um painel padrão do usuário 

Normalmente, você pode identificar um painel padrão do usuário definido se o botão **Definir como** padrão não aparecer na barra de comandos do painel. O painel padrão do usuário substituirá todos os outros painéis padrão, mesmo se o painel padrão do usuário não estiver no aplicativo atual.

Use a solução alternativa a seguir para desater seu painel padrão.

1. Crie um novo painel pessoal.

2. De definir esse novo painel como o padrão do usuário.

3. Exclua esse painel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O painel é definido no sitemap

Você pode ter definido um painel padrão da organização selecionando um painel e escolhendo "Definir como padrão" em "Personalizar o sistema". Mas o painel definido no designer de mapa de sites terá precedência sobre esse painel, se o usuário tiver acesso a ele.

Para que os usuários vejam o painel que você definiu como o padrão da organização, você pode:

* Definir esse painel no sitemap

* Remover o acesso ao painel definido do sitemap para esses usuários
