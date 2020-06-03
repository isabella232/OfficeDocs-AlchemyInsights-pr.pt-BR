---
title: Solucionando problemas de mensagens de acesso negado para sites do OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511172"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="74570-102">Solucionando problemas de mensagens de acesso negado para sites do OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="74570-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="74570-103">Esse problema ocorre com mais frequência quando um usuário é excluído e recriado com o mesmo nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="74570-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="74570-104">A nova conta é criada usando um valor diferente de PUID (ID exclusiva do Passport).</span><span class="sxs-lookup"><span data-stu-id="74570-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="74570-105">Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="74570-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="74570-106">Um segundo cenário envolve a sincronização de diretório com uma unidade organizacional (OU) do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="74570-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="74570-107">Se os usuários já tiverem entrado no SharePoint e forem movidos para uma OU diferente e ressincronizado com o SharePoint, poderão enfrentar esse problema.</span><span class="sxs-lookup"><span data-stu-id="74570-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="74570-108">Para resolver esse problema, você deve restaurar o UPN original com as etapas no artigo, [restaurar um usuário no Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="74570-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="74570-109">Se não for possível restaurar o usuário original, remova o usuário antigo do site do OneDrive usando estas etapas, [remova um usuário da lista de informações do usuário]().</span><span class="sxs-lookup"><span data-stu-id="74570-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="74570-110">Depois disso, você pode verificar se o usuário tem direitos de administrador para o site do OneDrive seguindo as etapas para [Adicionar o administrador do onedrive de um usuário](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="74570-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="74570-111">Para obter mais informações sobre níveis de permissão, confira o artigo [noções básicas sobre níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="74570-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
