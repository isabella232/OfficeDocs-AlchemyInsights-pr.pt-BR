---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812535"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="38c98-102">O Outlook não consegue se conectar a pastas públicas</span><span class="sxs-lookup"><span data-stu-id="38c98-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="38c98-103">Se o acesso à pasta pública não estiver funcionando para alguns usuários, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="38c98-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="38c98-104">Conecte-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário com problema para corresponder ao parâmetro em uma conta de usuário em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="38c98-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="38c98-105">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="38c98-105">Example:</span></span>

<span data-ttu-id="38c98-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="38c98-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="38c98-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="38c98-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="38c98-108">Aguarde pelo menos uma hora para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="38c98-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="38c98-109">Se o problema permanecer, siga [este procedimento](https://aka.ms/pfcte) para solucionar problemas de acesso à pasta pública usando o Outlook.</span><span class="sxs-lookup"><span data-stu-id="38c98-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="38c98-110">**Para controlar quais usuários podem acessar pastas públicas usando o Outlook**:</span><span class="sxs-lookup"><span data-stu-id="38c98-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="38c98-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false</span><span class="sxs-lookup"><span data-stu-id="38c98-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="38c98-112">$true: permitir que os usuários acessem pastas públicas no Outlook</span><span class="sxs-lookup"><span data-stu-id="38c98-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="38c98-113">$false: impedir que os usuários acessem pastas públicas no Outlook.</span><span class="sxs-lookup"><span data-stu-id="38c98-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="38c98-114">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="38c98-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="38c98-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="38c98-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="38c98-116">**Observação** Este procedimento só pode controlar conexões com o Outlook desktop para clientes Windows.</span><span class="sxs-lookup"><span data-stu-id="38c98-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="38c98-117">Um usuário pode continuar acessando pastas públicas usando o OWA ou o Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="38c98-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="38c98-118">Para obter mais informações, consulte [anunciando suporte para conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="38c98-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>