---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891737"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1166a-102">O Outlook não consegue se conectar a pastas públicas</span><span class="sxs-lookup"><span data-stu-id="1166a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1166a-103">Se o acesso à pasta pública não estiver funcionando para alguns usuários, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="1166a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="1166a-104">Conecte-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário com problema para corresponder ao parâmetro em uma conta de usuário em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="1166a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="1166a-105">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="1166a-105">Example:</span></span>

<span data-ttu-id="1166a-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="1166a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1166a-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valor de comando anterior></span><span class="sxs-lookup"><span data-stu-id="1166a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1166a-108">Aguarde pelo menos uma hora para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="1166a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="1166a-109">Se o problema permanecer, siga [este procedimento](https://aka.ms/pfcte) para solucionar problemas de acesso à pasta pública usando o Outlook.</span><span class="sxs-lookup"><span data-stu-id="1166a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>