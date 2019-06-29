---
title: Mover mensagens de email para a caixa de correio de arquivo morto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379485"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover email para a caixa de correio de arquivo morto

1. Confirmar se uma **caixa de correio de arquivo morto** foi habilitada. Caso contrário, use as etapas neste [artigo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) para habilitar a caixa de correio de arquivo morto.

2. Para arquivar mensagens automaticamente na caixa de correio de arquivo morto, uma marca de retenção com a ação **mover para arquivo morto** deve ser definida como **aplicada automaticamente à marca de caixa de correio inteira (padrão)**. Use as etapas aqui para criar a marca de formatação: [arquivo morto padrão](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Em seguida, adicione a marca **Archive** à sua política de retenção. No centro de administração do Exchange, escolha **políticas de retenção** > adicionar a **marca mover para arquivo morto** à política > **salvar**.

4. Agora, [atribua a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio do usuário específico. A mesma política será aplicada à caixa de correio **principal** e de **arquivo morto** .

Pode ser necessário forçar o assistente de pasta gerenciada (MFA) a ser executado e aplicar as novas configurações à caixa de correio do usuário. Execute o seguinte comando enquanto [estiver conectado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o assistente de pasta gerenciada para uma caixa de correio específica:
  
Start-ManagedFolderAssistant-Identity<name of the mailbox>

Para obter mais informações sobre como configurar uma política de arquivo morto, consulte [Configurar uma política de arquivo morto e exclusão para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  