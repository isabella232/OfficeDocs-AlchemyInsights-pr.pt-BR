---
title: Mover mensagens de email para a caixa de correio Arquivo morto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974945"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover email para a caixa de correio de arquivo morto

Se você quiser que executemos verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <-- na parte superior desta página e insira o endereço de email do usuário que tem problemas para mover emails para sua caixa de correio de arquivo morto.

1. Confirme se uma **caixa de correio De** arquivo morto foi habilitada. Caso não seja, use as etapas [deste artigo para](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) habilitar a caixa de correio de arquivo morto.

2. Para arquivar mensagens automaticamente na caixa de correio de arquivo morto, uma marca de retenção com a ação **Mover** para arquivo morto deve ser definida como aplicada automaticamente à marca de caixa de correio **inteira (padrão).** Use as etapas aqui para criar a marca: [Marca padrão de arquivo morto.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Em seguida, adicione a marca **Archive** à sua política de retenção. No centro Exchange de administração, escolha Políticas de **retenção** > adicionar a marca **Mover** para Arquivo morto à política > **Salvar**.

4. Agora [atribua a Política de Retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio do usuário específico. A mesma política será aplicada à caixa de correio **Primária** e **à Caixa de Correio de** Arquivo Morto.

Pode ser necessário forçar o Assistente de Pasta Gerenciada (MFA) a ser executado e aplicar as novas configurações à caixa de correio do usuário. Execute o seguinte comando enquanto [estiver conectado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pasta Gerenciada para uma caixa de correio específica:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Para obter mais informações sobre como configurar uma política de arquivo morto, consulte Configurar uma política de arquivamento e [exclusão para caixas de correio](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  