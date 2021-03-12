---
title: Criptografar automaticamente determinadas mensagens de email do Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735390"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Criptografar automaticamente determinadas mensagens de email do Office 365

Você pode criptografar automaticamente mensagens que os usuários enviam para determinadas pessoas ou organizações externas. Para fazer isso, execute as seguintes etapas:

1. No Centro [de administração do Exchange,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.** 
2. Clique no **ícone Novo (+)** e, em seguida, clique em Aplicar a Criptografia de Mensagens do **Office 365 e proteção de** direitos às mensagens .
3. Em **Nome**, insira um nome para a regra, como *Criptografar mensagens enviadas para DrToniRamos@gmail.com*.
4. In **Apply this rule if**, choose The recipient > is this **person**. 
5. Na janela **Selecionar Membros,** selecione o nome da pessoa à quem você deseja aplicar a regra de criptografia e clique em **adicionar**. 
6. Quando terminar de adicionar usuários, clique em **OK**.
7. Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**. 
8. No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**. (Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática. Mas você pode adicioná-lo!)
9. Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).
10. Clique em **Salvar**.

> [!IMPORTANT]
> Você sempre pode voltar e editar essa regra mais tarde.

Para obter mais informações sobre como criar regras para criptografia, consulte Definir regras de fluxo de emails para criptografar mensagens de [email no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

