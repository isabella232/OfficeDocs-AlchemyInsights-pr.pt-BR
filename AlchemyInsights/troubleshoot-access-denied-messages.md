---
title: Solucionar problemas de mensagens negadas do Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704882"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f91d1-102">Solucionar problemas de mensagens negadas do Access</span><span class="sxs-lookup"><span data-stu-id="f91d1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f91d1-103">Se alguém recebeu uma mensagem "Acesso Negado" para uma pasta compartilhada no SharePoint, o administrador do conjunto de sites pode ter habilitado o "modo de bloqueio de permissão de usuário de acesso limitado".</span><span class="sxs-lookup"><span data-stu-id="f91d1-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="f91d1-104">Para desativar isso:</span><span class="sxs-lookup"><span data-stu-id="f91d1-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="f91d1-105">Navegue até o site, clique no ícone Configurações e clique em **Configurações do Site.**</span><span class="sxs-lookup"><span data-stu-id="f91d1-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f91d1-106">Em **Administração do Conjunto de Sites**, clique em **Recursos do conjunto de sites**.</span><span class="sxs-lookup"><span data-stu-id="f91d1-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f91d1-107">Ao lado do modo de bloqueio de permissão de usuário de acesso **limitado,** clique **em Desativar**.</span><span class="sxs-lookup"><span data-stu-id="f91d1-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f91d1-108">Uma mensagem de Acesso Negado também pode ocorrer para pastas compartilhadas se o site for um site de publicação.</span><span class="sxs-lookup"><span data-stu-id="f91d1-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="f91d1-109">Para obter informações, [consulte Access Denied ao acessar uma pasta compartilhada](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="f91d1-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="f91d1-110">Se uma pessoa recebeu uma mensagem "Acesso Negado" ao tentar exibir solicitações de acesso, o usuário precisa ser adicionado como administrador de conjunto de sites ou membro do grupo Proprietários do site.</span><span class="sxs-lookup"><span data-stu-id="f91d1-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="f91d1-111">Para obter mais informações, [consulte Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f91d1-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f91d1-112">Se um usuário recebeu uma mensagem "Acesso Negado" depois que foi removido do Active Directory local e adicionado de volta, consulte Access Denied when a user account is [synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f91d1-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

