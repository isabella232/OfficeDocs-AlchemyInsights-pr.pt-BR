---
title: Solucionar problemas de mensagens de acesso negado
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500384"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f9ced-102">Solucionar problemas de mensagens de acesso negado</span><span class="sxs-lookup"><span data-stu-id="f9ced-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f9ced-103">Se alguém tiver uma mensagem de "acesso negado" para uma pasta compartilhada no SharePoint, o administrador do conjunto de sites poderá ter habilitado o "modo de bloqueio de permissão de usuário com acesso limitado".</span><span class="sxs-lookup"><span data-stu-id="f9ced-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="f9ced-104">Para desativá-la:</span><span class="sxs-lookup"><span data-stu-id="f9ced-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="f9ced-105">Navegue até o site, clique no ícone configurações e, em seguida, clique em **configurações do site**.</span><span class="sxs-lookup"><span data-stu-id="f9ced-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f9ced-106">Em **Administração do Conjunto de Sites**, clique em **Recursos do conjunto de sites**.</span><span class="sxs-lookup"><span data-stu-id="f9ced-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f9ced-107">Ao lado de **modo de bloqueio de permissão de usuário com acesso limitado**, clique em **desativar**.</span><span class="sxs-lookup"><span data-stu-id="f9ced-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f9ced-108">Uma mensagem de acesso negado também pode ocorrer para pastas compartilhadas se o site for um site de publicação.</span><span class="sxs-lookup"><span data-stu-id="f9ced-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="f9ced-109">Para obter informações, consulte [acesso negado ao acessar uma pasta compartilhada](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="f9ced-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="f9ced-110">Se uma pessoa receber uma mensagem de "acesso negado" ao tentar exibir solicitações de acesso, o usuário precisará ser adicionado como um administrador de conjunto de sites ou membro do grupo de proprietários do site.</span><span class="sxs-lookup"><span data-stu-id="f9ced-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="f9ced-111">Para obter mais informações, consulte [acesso negado à lista de solicitações de acesso](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f9ced-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f9ced-112">Se um usuário tiver uma mensagem de "acesso negado" após ter sido removida do Active Directory local e adicionado novamente, confira [acesso negado quando uma conta de usuário for sincronizada com o Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f9ced-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

