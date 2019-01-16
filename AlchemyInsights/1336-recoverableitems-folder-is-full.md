---
title: Pasta de RecoverableItems 1336 está cheio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274621"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta itens recuperáveis está cheio

Para caixas de correio Exchange Online no Office 365, o limite de armazenamento padrão para a pasta itens recuperáveis é 30 GB. O limite de armazenamento para a pasta itens recuperáveis automaticamente é aumentado para 100 GB se a caixa de correio for colocada em retenção de litígio, retenção de descoberta eletrônica ou é atribuída a uma política de retenção do Office 365.
  
Quando a pasta itens recuperáveis atinge o limite de armazenamento, a funcionalidade de caixa de correio é afetada das seguintes maneiras:
  
- O usuário não pode excluir itens da caixa de correio.
    
- O Assistente de Pasta Gerenciada não pode excluir itens com base na marca de retenção ou nas configurações de pasta gerenciada.
    
- Para caixas de correio que tenham a recuperação de Item único habilitada ou são colocadas em espera, o processo de proteção de página de cópia-na-gravação não pode manter versões dos itens editados pelo usuário.
    
- Para caixas de correio que tem a caixa de correio habilitada de log de auditoria, nenhuma entrada de log de auditoria de caixa de correio pode ser salvas na subpasta auditorias na pasta itens recuperáveis.
    
Para caixas de correio que não estão em espera, os administradores podem usar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command no PowerShell do Exchange Online para excluir itens na pasta itens recuperáveis. Para obter mais informações, consulte os tópicos a seguir: 
  
- [Procurar e excluir mensagens](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Para caixas de correio que estiverem em espera, os administradores precisa remover a retenção antes que eles podem itens excluídos da pasta itens recuperáveis. Para obter mais informações, consulte [Excluir itens na pasta de caixas de correio baseadas em nuvem em espera itens recuperáveis](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Para ajudar a evitar que a pasta itens recuperáveis se torne completa, os administradores podem aumentar o limite de armazenamento dos itens recuperáveis pasta para caixas de correio em espera e definir uma política de retenção de caixa de correio que move itens da pasta itens recuperáveis para o arquivo do usuário caixa de correio. Consulte [aumentar a cota de caixas de correio em retenção de itens recuperáveis](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

