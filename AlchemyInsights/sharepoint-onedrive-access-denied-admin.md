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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707942"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="80106-102">Solucionar problemas de acesso mensagens negadas no Centro de Administração do Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="80106-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="80106-103">Se você estiver recebendo uma mensagem de acesso negado ao tentar navegar até um Centro de Administração do Sharepoint/OneDrive, certifique-se de atribuir uma licença [ao usuário](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="80106-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="80106-104">Se o usuário tiver uma licença, você [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) também deverá garantir que ele tenha uma função de administrador que possa acessar os centros de administração.</span><span class="sxs-lookup"><span data-stu-id="80106-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="80106-105">Esse problema também pode ocorrer quando um usuário é excluído e re-criado com o mesmo nome de entidade de usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="80106-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="80106-106">A nova conta é criada usando um valor puid diferente (ID exclusiva do Passport).</span><span class="sxs-lookup"><span data-stu-id="80106-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="80106-107">Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="80106-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="80106-108">Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (UO).</span><span class="sxs-lookup"><span data-stu-id="80106-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="80106-109">Se os usuários já entraram no SharePoint e, em seguida, são movidos para uma OU diferente e reanciados com o SharePoint, eles podem ter esse problema.</span><span class="sxs-lookup"><span data-stu-id="80106-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="80106-110">Para resolver esse problema, você deve restaurar o UPN original com as etapas do artigo, Restaurar um usuário [no Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="80106-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="80106-111">Observação: se um Centro de Administração do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="80106-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="80106-112">[Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="80106-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


