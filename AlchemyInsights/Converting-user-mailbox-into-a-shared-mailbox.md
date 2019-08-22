---
title: Convertendo caixa de correio do usuário em uma caixa de correio compartilhada?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496387"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Converter uma caixa de correio do usuário em uma caixa de correio compartilhada

Você só pode converter uma caixa de correio de usuário em uma caixa de correio compartilhada se o usuário tiver uma licença do Exchange. Depois que a caixa de correio é convertida, ela continuará a aparecer na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas. No entanto, a caixa de correio convertida também será exibida na lista de caixas de correio compartilhadas. 
  
Se você tentar converter uma caixa de correio no console de administração do Exchange e a conversão falhar, limpe o cache do navegador e os cookies e tente novamente. Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:
  
```
Set-Mailbox -Type Shared
```

Mais informações de conversão de caixa de correio estão disponíveis em [converter uma caixa de correio de usuário para uma caixa de correio compartilhada](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
