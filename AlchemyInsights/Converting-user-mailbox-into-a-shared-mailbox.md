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
<span data-ttu-id="92a05-102">Você só pode converter uma caixa de correio de usuário em uma caixa de correio compartilhada se o usuário tiver uma licença do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92a05-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="92a05-103">Depois que a caixa de correio é convertida, ela continuará a aparecer na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="92a05-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="92a05-104">No enTanto, a caixa de correio convertida também será exibida na lista de caixas de correio compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="92a05-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="92a05-105">Se você tentar converter uma caixa de correio no console de administração do Exchange e a conversão falhar, limpe o cache do navegador e os cookies e tente novamente.</span><span class="sxs-lookup"><span data-stu-id="92a05-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="92a05-106">Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="92a05-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="92a05-107">Mais informações de conversão de caixa de correio estão disponíveis em [converter uma caixa de correio de usuário para uma caixa de correio compartilhada](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="92a05-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
