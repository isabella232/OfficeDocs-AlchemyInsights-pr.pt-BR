---
title: 305 aumentar o tamanho da caixa de correio de arquivo morto
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
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778571"
---
# <a name="increase-the-archive-mailbox-size"></a>Aumentar o tamanho da caixa de correio de arquivo morto


Se você quiser executar verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <-no início desta página e insira o endereço de email do usuário que precisa de seu tamanho de caixa de correio de arquivo.

A Microsoft 365 [limita](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) o tamanho das caixas de correio de arquivo morto com base na licença atribuída à conta de usuário. Quando a caixa de correio de arquivo morto alcança 90% de seu tamanho permitido, o usuário recebe uma notificação por email. Quando uma caixa de correio de arquivo morto atinge seu limite de tamanho, o usuário não pode mover mais itens para a caixa de correio de arquivo morto. O Microsoft 365 não aumentará o tamanho de uma caixa de correio de arquivo morto quando o limite de tamanho for atingido. Em vez disso, os usuários podem executar as seguintes ações para liberar espaço na caixa de correio de arquivo morto:

- Exporte os itens para um arquivo. pst usando o Outlook.

- Excluir itens da caixa de correio de arquivo morto.

O Microsoft 365 fornece **arquivamento ilimitado** para as licenças do Office 365 Enterprise E3 e e5. Um administrador deve habilitar esse recurso antes que a caixa de correio de arquivo morto alcance o tamanho máximo. Quando o arquivamento ilimitado é habilitado, pode levar até 30 dias antes de o espaço livre ser adicionado à caixa de correio de arquivo morto. Portanto, recomendamos que os administradores verifiquem o espaço livre na caixa de correio de arquivo morto, permitindo que o usuário continue usando a caixa de correio de arquivo morto enquanto expande. Para obter mais informações, consulte [Overview of Unlimited Archiving in microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) e [Enable Unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Para obter mais informações sobre como acessar a caixa de correio de arquivo morto no Outlook, confira [requisitos do Outlook para acessar itens em um arquivo morto expandido automaticamente](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Para configurar uma política de retenção que move automaticamente itens para a caixa de correio de arquivo morto, consulte [Configurar uma política de arquivo morto e exclusão para caixas de correio em sua organização do Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Observação**: a expansão automática de arquivos não é suportada para caixas de correio principais no Exchange 2010.
