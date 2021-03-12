---
title: Mover automaticamente mensagens de email para a caixa de correio de arquivo morto
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735378"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mover automaticamente mensagens de email para a caixa de correio de arquivo morto

Veja como configurar uma política para mover automaticamente o email antigo de um usuário para a caixa de correio de arquivo morto:

1. Acesse [**Security & Compliance Data**](https://go.microsoft.com/fwlink/p/?linkid=2077143)governance Archive para verificar se uma caixa de correio de arquivo morto  >    >   foi habilitada para o usuário. Se não tiver, clique em **Habilitar,** **em seguida, Sim** na caixa de aviso.
2. Vá para o [**Centro de administração do Exchange > gerenciamento de conformidade > marcas de retenção**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Escolha o ícone + e escolha **aplicar automaticamente a caixa de correio inteira.**
4. Atribua um nome à marca de retenção e escolha **Mover para Arquivar**. Para o período de retenção, insira o tempo que você deseja, como 90 dias. Clique em **Salvar**.
5. Agora crie uma política de retenção: escolha **políticas de** retenção , escolha o ícone para adicionar uma nova política.
6. Atribua um nome à política de retenção e clique e role para encontrar e adicionar a marca de retenção que você acabou de criar. Clique em **Salvar**.
7. Por fim, aplique a política de retenção à caixa de correio do usuário: ainda no Centro de administração do Exchange, vá para caixas **de** correio  >  **de destinatários.** Escolha todos os usuários aos quais você deseja aplicar a política e escolha **Editar** (o ícone do lápis).
8. Na caixa de diálogo, clique em recursos **de caixa de correio**. Em **Política de retenção,** aplique a política que você acabou de criar > **Salvar**.
9. Para obter instruções para aplicar a política a todos os usuários, consulte [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
