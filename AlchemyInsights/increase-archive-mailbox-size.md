---
title: 305 Aumentar o tamanho da caixa de correio de arquivo morto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926371"
---
# <a name="increase-the-archive-mailbox-size"></a>Aumentar o tamanho da caixa de correio de arquivo morto


Se você quiser que executemos verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <-- na parte superior desta página e insira o endereço de email do usuário que precisa aumentar o tamanho da caixa de correio de arquivo morto.

Microsoft 365 limita [o](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) tamanho das caixas de correio de arquivo morto com base na licença atribuída à conta de usuário. Quando a caixa de correio de arquivo morto atinge 90% do tamanho permitido, o usuário recebe uma notificação por email. Quando uma caixa de correio de arquivo morto atinge seu limite de tamanho, o usuário não pode mover mais itens para a caixa de correio de arquivo morto. Microsoft 365 aumentará o tamanho de uma caixa de correio de arquivo morto depois que o limite de tamanho for atingido. Em vez disso, os usuários podem tomar as seguintes ações para liberar espaço na caixa de correio de arquivo morto:

- Exporte os itens para um arquivo .pst usando Outlook.

- Exclua itens da caixa de correio de arquivo morto.

Microsoft 365 fornece **arquivamento ilimitado** para licenças Office 365 Enterprise E3 e E5. Um administrador deve habilitar esse recurso antes que a caixa de correio de arquivo morto atinja seu tamanho máximo. Quando o arquivamento ilimitado é habilitado, pode levar até 30 dias para que o espaço livre seja adicionado à caixa de correio de arquivo morto. Portanto, recomendamos que os administradores verifiquem o espaço livre na caixa de correio de arquivo morto, o que permite que o usuário continue usando a caixa de correio de arquivo morto enquanto ela se expande. Para obter mais informações, consulte [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and Enable unlimited [archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Para obter mais informações sobre como acessar a caixa de correio de arquivo morto Outlook, consulte Outlook requisitos para acessar itens em um arquivo morto [expandido automaticamente.](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) Para configurar uma política de retenção que move automaticamente itens para a caixa de correio de arquivo morto, consulte Configurar uma política de arquivamento e exclusão para caixas de correio em sua organização [Microsoft 365.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**Observação:** arquivos de expansão automática não são suportados para caixas de correio principais no Exchange 2010.
