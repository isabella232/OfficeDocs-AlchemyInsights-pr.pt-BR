---
title: Comportamento ConsistencyGuid/atributo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705721"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="83186-102">Comportamento ConsistencyGuid/atributo</span><span class="sxs-lookup"><span data-stu-id="83186-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="83186-103">O Azure AD Connect (versão 1.1.524.0 e posterior) agora facilita o uso do atributo msDS-ConsistencyGuid as atributo.</span><span class="sxs-lookup"><span data-stu-id="83186-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="83186-104">Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="83186-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="83186-105">Use msDS-ConsistencyGuid como o atributo atributo para objetos de usuário.</span><span class="sxs-lookup"><span data-stu-id="83186-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="83186-106">ObjectGUID é usado para outros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="83186-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="83186-107">Para qualquer objeto de usuário do AD local específico cujo atributo msDS-ConsistencyGuid não esteja preenchido, o Azure AD Connect grava seu valor objectGUID de volta para o atributo msDS-ConsistencyGuid no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="83186-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="83186-108">Após o atributo msDS-ConsistencyGuid ser preenchido, o Azure AD Connect, exporta o objeto para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="83186-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="83186-109">**Observação:** Depois que um objeto do AD local é importado para o Azure AD Connect (ou seja, importado para o espaço do conector do AD e projetado para o metaverso), você não pode mais alterar o valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="83186-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="83186-110">Para especificar o valor de atributo para um determinado objeto AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="83186-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="83186-111">Para obter mais informações sobre o atributo e o ConsistencyGuid, consulte o seguinte: [Azure ad Connect: design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="83186-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

