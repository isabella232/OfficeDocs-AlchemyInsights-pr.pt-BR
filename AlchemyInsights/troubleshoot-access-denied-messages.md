---
title: Solucionar problemas de mensagens de acesso negado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759788"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="4d58a-102">Solucionar problemas de mensagens de acesso negado</span><span class="sxs-lookup"><span data-stu-id="4d58a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="4d58a-103">Se alguém tiver uma mensagem de "acesso negado" para uma pasta compartilhada no SharePoint, o administrador do conjunto de sites poderá ter habilitado o "modo de bloqueio de permissão de usuário com acesso limitado".</span><span class="sxs-lookup"><span data-stu-id="4d58a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="4d58a-104">Para desativá-la:</span><span class="sxs-lookup"><span data-stu-id="4d58a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="4d58a-105">Navegue até o site, clique no ícone configurações e, em seguida, clique em **configurações do site**.</span><span class="sxs-lookup"><span data-stu-id="4d58a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="4d58a-106">Em **Administração do Conjunto de Sites**, clique em **Recursos do conjunto de sites**.</span><span class="sxs-lookup"><span data-stu-id="4d58a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="4d58a-107">Ao lado de **modo de bloqueio de permissão de usuário com acesso limitado**, clique em **desativar**.</span><span class="sxs-lookup"><span data-stu-id="4d58a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="4d58a-108">Uma mensagem de acesso negado também pode ocorrer para pastas compartilhadas se o site for um site de publicação.</span><span class="sxs-lookup"><span data-stu-id="4d58a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="4d58a-109">Para obter informações, consulte [acesso negado ao acessar uma pasta compartilhada](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="4d58a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="4d58a-110">Se uma pessoa receber uma mensagem de "acesso negado" ao tentar exibir solicitações de acesso, o usuário precisará ser adicionado como um administrador de conjunto de sites ou membro do grupo de proprietários do site.</span><span class="sxs-lookup"><span data-stu-id="4d58a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="4d58a-111">Para obter mais informações, consulte [acesso negado à lista de solicitações de acesso](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="4d58a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="4d58a-112">Se um usuário tiver uma mensagem de "acesso negado" após ter sido removida do Active Directory local e adicionado novamente, confira [acesso negado quando uma conta de usuário for sincronizada com o Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="4d58a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

