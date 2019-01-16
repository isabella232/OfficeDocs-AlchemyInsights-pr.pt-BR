---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274729"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="56006-102">Quando as alterações do meu perfil sincronizar o aplicativo de perfil de usuário do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="56006-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="56006-103">SharePoint Online usa o trabalho de timer de importação do Active Directory (AD importar) para importar usuários e grupos para o aplicativo de perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="56006-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="56006-p101">Importação do AD sincroniza as alterações do repositório de diretório do SharePoint Online para o aplicativo de perfil de usuário. Essas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="56006-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="56006-106">O trabalho de timer é executado até que as alterações são sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="56006-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="56006-p102">O tempo que leva para executar o trabalho depende do número de alterações para processar. Um grande número de alterações é mais demorado. O contrato de nível de serviço (SLA) afirma que uma alteração em um usuário no SharePoint Online Directory será refletida no aplicativo de perfil de usuário em 24 horas.</span><span class="sxs-lookup"><span data-stu-id="56006-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="56006-110">Mais informações sobre a sincronização de perfil do usuário no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="56006-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

