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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="9d08d-102">Converter uma caixa de correio do usuário em uma caixa de correio compartilhada</span><span class="sxs-lookup"><span data-stu-id="9d08d-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="9d08d-103">Você só pode converter uma caixa de correio de usuário em uma caixa de correio compartilhada se o usuário tiver uma licença do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d08d-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="9d08d-104">Depois que a caixa de correio é convertida, ela continuará a aparecer na lista de usuários ativos porque essa lista inclui caixas de correio compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="9d08d-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="9d08d-105">No entanto, a caixa de correio convertida também será exibida na lista de caixas de correio compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="9d08d-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="9d08d-106">Se você tentar converter uma caixa de correio no console de administração do Exchange e a conversão falhar, limpe o cache do navegador e os cookies e tente novamente.</span><span class="sxs-lookup"><span data-stu-id="9d08d-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="9d08d-107">Se ainda não estiver funcionando, tente converter a caixa de correio no Shell de gerenciamento do Exchange executando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="9d08d-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="9d08d-108">Mais informações de conversão de caixa de correio estão disponíveis em [converter uma caixa de correio de usuário para uma caixa de correio compartilhada](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9d08d-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
