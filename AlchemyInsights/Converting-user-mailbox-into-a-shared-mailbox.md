---
title: Convertendo caixas de correio do usuário em uma caixa de correio compartilhada?
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906720"
---
Você só pode converter uma caixa de correio do usuário para uma caixa de correio compartilhada se o usuário possui uma licença do Exchange. Depois que a caixa de correio é convertida, ele continuará a mostrada na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas. No entanto, a caixa de correio convertida também serão exibidas na lista de caixa de correio compartilhada. 
  
Se você tentar converter uma caixa de correio no Console de administração do Exchange e a conversão falhar, desmarque os cookies e o cache do navegador e tente novamente. Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:
  
```
Set-Mailbox -Type Shared
```

Mais informações sobre conversão de caixa de correio está disponível no [converter uma caixa de correio do usuário para uma caixa de correio compartilhada](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
