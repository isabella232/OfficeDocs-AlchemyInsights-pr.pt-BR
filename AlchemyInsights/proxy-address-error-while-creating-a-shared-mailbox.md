---
title: Erro de endereço proxy ao criar uma caixa de correio compartilhada
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062896"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Erro de endereço proxy ao criar uma caixa de correio ou outro objeto habilitado para email

Se você tentou criar um objeto habilitado para email (caixa de correio, caixa de correio compartilhada etc.) e recebeu o erro "O endereço proxy "SMTP:alias@domain.com" já está sendo usado...", o endereço de email escolhido já será tomado por outro objeto habilitado para email em sua organização.
  
Você precisa encontrar o usuário, grupo, caixa de correio compartilhada ou pasta pública que tenha esse endereço de email e excluí-lo ou alterar seu endereço de email. Em seguida, você pode criar um novo objeto habilitado para email com o endereço de email liberado. Use a Pesquisa na Página Inicial para encontrá-la. Você também pode usar o seguinte comando Exchange Online PowerShell para pesquisá-lo:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Se você não quiser excluir o endereço de email existente, escolha um novo endereço de email para o novo objeto que você está criando.
  