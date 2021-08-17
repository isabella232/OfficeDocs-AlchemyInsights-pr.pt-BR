---
title: Corrigir política de conexão
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314832"
---
# <a name="fix-connection-policy"></a>Corrigir política de conexão

O email foi marcado como seguro e entregue à Caixa de Entrada do usuário porque o endereço IP de origem foi marcado como seguro na política de filtro de conexão padrão. Para revisar a política, faça as seguintes etapas:

1. No portal Microsoft 365 Defender , acesse Email & Políticas de Colaboração & Políticas de Ameaças de Regras <https://security.microsoft.com/>  \>  \>  \> **Anti-spam** na **seção** Políticas.

   Para ir diretamente à página de **Políticas antispam**, use <https://security.microsoft.com/antispam>.

2. Na página **Políticas anti-spam,** selecione a política denominada Política de filtro de **conexão (Padrão)** clicando no nome da política.

3. No sobremenu de detalhes exibido, clique em Editar política de filtro **de conexão** na seção **Filtragem de** conexão.

4. Revise as entradas na seção **Sempre permitir** mensagens da seção de endereços IP ou intervalo de endereços a seguir e veja se Ativar **lista segura** está selecionada.

   **Observação**: a Microsoft se inscreve em fontes de terceiros de senders confiáveis. Se a lista segura estiver habilitada, esses remetentes confiáveis não são marcados erroneamente como spam. Recomendamos selecionar essa opção, pois ela reduzirá o número de falsos positivos (emails bons que são classificados como spam) que você recebe.

Para obter mais informações, confira [Configurar a filtragem da conexão](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
