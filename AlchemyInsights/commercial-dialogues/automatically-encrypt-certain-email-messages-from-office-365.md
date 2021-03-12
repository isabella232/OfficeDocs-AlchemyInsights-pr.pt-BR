---
title: Criptografar automaticamente determinadas mensagens de email do office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735391"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Criptografar automaticamente determinadas mensagens de email do office 365

1. No Centro [de administração do Exchange,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.** 
2. Clique no **ícone Novo (+)** e, em seguida, clique em Aplicar a Criptografia de Mensagens do **Office 365 e proteção de** direitos às mensagens .
3. Em **Nome**, insira um nome para a regra, como *Criptografar todas as mensagens*.
4. Em **Aplicar essa regra se**, escolha **[Aplicar a todas as mensagens]**. 
5. Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**. 
6. No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**. (Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática. Mas você pode adicioná-lo!)
7. Marque a **caixa de seleção Auditar** essa regra com nível de gravidade e selecione o nível desejado. Se sua empresa tiver obrigações contratuais para enviar todos os emails criptografados, recomendamos definir o nível como **Alto**.
8. Em **Escolher um modelo para essa regra,** clique em **Impor**. 
9. Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).
10. Clique em **Salvar**.

> [!IMPORTANT]
> Você sempre pode voltar e editar essa regra mais tarde.

Para obter mais informações sobre como criar regras para criptografia, consulte Definir regras de fluxo de emails [para criptografar mensagens de email no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

