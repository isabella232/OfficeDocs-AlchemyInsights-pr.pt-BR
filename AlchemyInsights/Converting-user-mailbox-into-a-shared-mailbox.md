---
title: Convertendo caixas de correio do usuário em uma caixa de correio compartilhada?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456868"
---
<span data-ttu-id="4e84d-p101">Você só pode converter uma caixa de correio do usuário para uma caixa de correio compartilhada se o usuário possui uma licença do Exchange. Depois que a caixa de correio é convertida, ele continuará a mostrada na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas. No entanto, a caixa de correio convertida também serão exibidas na lista de caixa de correio compartilhada.</span><span class="sxs-lookup"><span data-stu-id="4e84d-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="4e84d-p102">Se você tentar converter uma caixa de correio no Console de administração do Exchange e a conversão falhar, desmarque os cookies e o cache do navegador e tente novamente. Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="4e84d-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="4e84d-107">Mais informações sobre conversão de caixa de correio está disponível no [converter uma caixa de correio do usuário para uma caixa de correio compartilhada](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="4e84d-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
