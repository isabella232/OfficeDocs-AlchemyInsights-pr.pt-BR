---
title: 1336 a pasta RecoverableItems está cheia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720240"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta itens recuperáveis está cheia

Para caixas de correio do Exchange Online, o limite de armazenamento padrão para a pasta itens recuperáveis é de 30 GB. O limite de armazenamento da pasta itens recuperáveis é aumentado automaticamente para 100 GB se a caixa de correio for colocada em retenção de litígio, retenção de descoberta eletrônica ou atribuída a uma política de retenção.

Quando a pasta itens recuperáveis atinge o limite de armazenamento, a funcionalidade de caixa de correio é afetada das seguintes maneiras:

- O usuário não pode excluir itens da caixa de correio.

- O Assistente de Pasta Gerenciada não pode excluir itens com base na marca de retenção ou nas configurações de pasta gerenciada.

- Para caixas de correio que têm a recuperação de item único habilitada ou são colocadas em espera, o processo de proteção de página de cópia de gravação não pode manter versões de itens editadas pelo usuário.

- Para caixas de correio com registro em log de auditoria de caixa de correio habilitado, nenhuma entrada de log de auditoria de caixa de correio pode ser salva na subpasta auditorias da pasta itens recuperáveis.

Para caixas de correio que não estão em retenção, os administradores `Search-Mailbox -SearchDumpsterOnly -DeleteContent` podem usar o comando no PowerShell do Exchange Online para excluir itens na pasta itens recuperáveis. Para mais informações, confira os seguintes tópicos:

- [Procurar e excluir mensagens](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para caixas de correio em espera, os administradores precisam remover a retenção antes de poderem excluir itens da pasta itens recuperáveis. Para obter mais informações, consulte [excluir itens na pasta itens recuperáveis de caixas de correio baseadas em nuvem em espera](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Para ajudar a evitar que a pasta de itens recuperáveis fique cheia, os administradores podem aumentar o limite de armazenamento da pasta itens recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixa de correio que move itens da pasta itens recuperáveis para a caixa de correio de arquivo morto do usuário. Consulte [aumentar a cota de itens recuperáveis para caixas de correio em espera](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
