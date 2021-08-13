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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988070"
---
# <a name="fix-connection-policy"></a>Corrigir política de conexão

O email foi marcado como seguro e entregue à caixa de entrada do usuário porque o endereço IP de envio foi marcado como seguro na política filtro de conexão. Para revisar a política, faça o seguinte:

1. Vá para o [Centro Office 365 Segurança & Conformidade](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para **Política** de Gerenciamento de Ameaças  >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na guia **Personalizado,** selecione a política de filtro **de conexão** e selecione **Editar política**.
3. Revise a **lista de IDS.** Veja se **Cofre lista** está habilitada.

    > [!NOTE]
    > A Microsoft assina fontes terceirizadas de remetentes confiáveis. Se **Cofre lista** estiver habilitada, esses remetentes confiáveis não são marcados erroneamente como spam. É recomendável selecionar essa opção, pois ela reduzirá o número de falsos positivos (emails que são classificados como spam) que você recebe.
