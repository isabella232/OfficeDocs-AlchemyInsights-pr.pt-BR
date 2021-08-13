---
title: 1336 Pasta RecoverableItems está cheia
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061744"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta Itens Recuperáveis está cheia

Para Exchange Online caixas de correio, o limite de armazenamento padrão para a pasta Itens Recuperáveis é 30 GB. O limite de armazenamento para a pasta Itens Recuperáveis é automaticamente aumentado para 100 GB se a caixa de correio for colocada em Retenção de Litígio, Retenção de Descoberta Automática ou for atribuída a uma política de retenção.

Quando a pasta Itens Recuperáveis atinge o limite de armazenamento, a funcionalidade da caixa de correio é afetada das seguintes maneiras:

- O usuário não pode excluir itens da caixa de correio.

- O Assistente de Pasta Gerenciada não pode excluir itens com base na marca de retenção ou nas configurações de pasta gerenciada.

- Para caixas de correio que tenham a Recuperação de Item Único habilitada ou colocadas em espera, o processo de proteção de página de cópia na gravação não pode manter versões de itens editados pelo usuário.

- Para caixas de correio que tenham o log de auditoria de caixa de correio habilitado, nenhuma entrada de log de auditoria de caixa de correio pode ser salva na subpasta Auditorias na pasta Itens Recuperáveis.

Para caixas de correio que não estão em espera, os administradores podem usar o comando no Exchange Online PowerShell para excluir itens na `Search-Mailbox -SearchDumpsterOnly -DeleteContent` pasta Itens Recuperáveis. Para mais informações, confira os seguintes tópicos:

- [Procurar e excluir mensagens](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para caixas de correio que estão em espera, os administradores precisam remover a responsabilidade antes que eles possam excluir itens da pasta Itens Recuperáveis. Para obter mais informações, consulte Excluir itens na pasta Itens Recuperáveis de caixas [de correio baseadas em nuvem em espera](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Para ajudar a impedir que a pasta Itens Recuperáveis se torne completa, os administradores podem aumentar o limite de armazenamento da pasta Itens Recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixa de correio que move itens da pasta Itens Recuperáveis para a caixa de correio de arquivo morto do usuário. Consulte [Aumentar a cota de Itens Recuperáveis para caixas de correio em espera.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
