---
title: Excluir um usuário órfão do servidor local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680123"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="c5abf-102">Excluir um usuário órfão do servidor local</span><span class="sxs-lookup"><span data-stu-id="c5abf-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="c5abf-103">Para remover um usuário órfão, siga as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="c5abf-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="c5abf-104">Force a sincronização de diretórios seguindo as instruções do artigo [O que é identidade híbrida com o Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="c5abf-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="c5abf-105">Para verificar a sincronização de diretórios, confira o artigo [O que é identidade híbrida com o Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="c5abf-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="c5abf-106">Se a sincronização funcionar corretamente, mas a exclusão do objeto Active Directory não for propagada para o Azure AD, remova manualmente o objeto órfão usando um dos seguintes cmdlets do Azure Active Directory para o Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c5abf-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="c5abf-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="c5abf-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="c5abf-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="c5abf-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="c5abf-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="c5abf-109">Remove-MsolUser</span></span>

    <span data-ttu-id="c5abf-110">Por exemplo, para remover a ID do usuário órfão john.smith@contoso.com, criada originalmente usando a sincronização de diretórios, execute o cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c5abf-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="c5abf-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="c5abf-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>