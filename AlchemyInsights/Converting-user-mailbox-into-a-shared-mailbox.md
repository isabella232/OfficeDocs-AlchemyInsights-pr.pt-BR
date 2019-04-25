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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374311"
---
Você só pode converter uma caixa de correio de usuário em uma caixa de correio compartilhada se o usuário tiver uma licença do Exchange. Depois que a caixa de correio é convertida, ela continuará a aparecer na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas. No enTanto, a caixa de correio convertida também será exibida na lista de caixas de correio compartilhadas. 
  
Se você tentar converter uma caixa de correio no console de administração do Exchange e a conversão falhar, limpe o cache do navegador e os cookies e tente novamente. Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:
  
```
Set-Mailbox -Type Shared
```

Mais informações de conversão de caixa de correio estão disponíveis em [converter uma caixa de correio de usuário para uma caixa de correio compartilhada](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
