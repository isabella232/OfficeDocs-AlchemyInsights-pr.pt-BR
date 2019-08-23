---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554321"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5e32c-102">Quando o meu perfil é alterado, sincronizar com o aplicativo de perfil de usuário do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="5e32c-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5e32c-103">O SharePoint Online usa o trabalho de timer de importação do Active Directory (AD Import) para importar usuários e grupos para o aplicativo de perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="5e32c-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5e32c-104">A importação do AD sincroniza as alterações do repositório de diretórios do SharePoint Online para o aplicativo de perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="5e32c-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="5e32c-105">Essas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="5e32c-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5e32c-106">O trabalho de timer é executado até que as alterações sejam sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="5e32c-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5e32c-107">O tempo necessário para a execução do trabalho depende do número de alterações a serem processadas.</span><span class="sxs-lookup"><span data-stu-id="5e32c-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="5e32c-108">Um grande número de alterações demora mais.</span><span class="sxs-lookup"><span data-stu-id="5e32c-108">A large number of changes takes longer.</span></span> <span data-ttu-id="5e32c-109">O contrato de nível de serviço (SLA) informa que uma alteração em um usuário no diretório do SharePoint Online será refletida no aplicativo de perfil de usuário em 24 horas.</span><span class="sxs-lookup"><span data-stu-id="5e32c-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5e32c-110">Mais informações sobre a sincronização de perfil de usuário no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5e32c-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

