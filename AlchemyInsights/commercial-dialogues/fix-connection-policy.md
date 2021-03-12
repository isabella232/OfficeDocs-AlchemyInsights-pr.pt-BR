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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735685"
---
# <a name="fix-connection-policy"></a>Corrigir política de conexão

O email foi marcado como seguro e entregue à caixa de entrada do usuário porque o endereço IP de envio foi marcado como seguro na política filtro de conexão. Para revisar a política, faça o seguinte:

1. Vá para o Centro de Conformidade e Segurança [& do Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para Política de Gerenciamento de Ameaças   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na guia **Personalizado,** selecione a política de filtro **de conexão** e selecione **Editar política**.
3. Revise a **lista de IDS.** Veja se **a lista segura** está habilitada.

    > [!NOTE]
    > A Microsoft assina fontes terceirizadas de remetentes confiáveis. Se **a lista segura** estiver habilitada, esses remetentes confiáveis não são marcados erroneamente como spam. É recomendável selecionar essa opção, pois ela reduzirá o número de falsos positivos (emails que são classificados como spam) que você recebe.
