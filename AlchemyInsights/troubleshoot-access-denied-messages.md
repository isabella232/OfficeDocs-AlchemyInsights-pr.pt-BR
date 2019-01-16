---
title: Solucionar mensagens de acesso negado
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274908"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d7470-102">Solucionar mensagens de acesso negado</span><span class="sxs-lookup"><span data-stu-id="d7470-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d7470-p101">Se alguém receber uma mensagem de "Acesso negado" para uma pasta compartilhada, o administrador do conjunto de sites pode ter ativado "modo de acesso limitado usuário permissão bloqueio". Para desativar isso:</span><span class="sxs-lookup"><span data-stu-id="d7470-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="d7470-105">Navegue até o site, clique no ícone configurações e, em seguida, clique em **Configurações do Site**.</span><span class="sxs-lookup"><span data-stu-id="d7470-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d7470-106">Em **Administração do Conjunto de Sites**, clique em **Recursos do conjunto de sites**.</span><span class="sxs-lookup"><span data-stu-id="d7470-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d7470-107">Ao lado de **modo de bloqueio de permissão de usuário de acesso limitado**, clique em **Desativar**.</span><span class="sxs-lookup"><span data-stu-id="d7470-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d7470-p102">Uma mensagem acesso negado também pode ocorrer para pastas compartilhadas, se o site for um site de publicação. Para informações, consulte [Acesso negado ao acessar uma pasta compartilhada](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="d7470-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="d7470-p103">Se um alguém receber uma mensagem de "Acesso negado" ao tentar visualizar as solicitações de acesso, o usuário precisa ser adicionado como um administrador de conjunto de sites ou um membro do grupo de proprietários do site. Para obter mais informações, consulte [Acesso negado à lista de solicitações de acesso](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="d7470-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d7470-112">Se um usuário receber uma mensagem de "Acesso negado" depois que eles foram removidos do Active Directory local e são adicionados novamente, consulte [Acesso negado quando uma conta de usuário é sincronizada com o Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="d7470-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

