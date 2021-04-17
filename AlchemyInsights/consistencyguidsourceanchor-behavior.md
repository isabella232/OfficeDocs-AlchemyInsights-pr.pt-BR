---
title: Comportamento consistencyGuid /sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816980"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="15d29-102">Comportamento consistencyGuid /sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="15d29-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="15d29-103">O Azure AD Connect (versão 1.1.524.0 e depois) agora facilita o uso do msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="15d29-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="15d29-104">Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="15d29-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="15d29-105">Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User.</span><span class="sxs-lookup"><span data-stu-id="15d29-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="15d29-106">ObjectGUID é usado para outros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="15d29-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="15d29-107">Para qualquer determinado objeto usuário do AD local cujo atributo msDS-ConsistencyGuid não está preenchido, o Azure AD Connect grava seu valor objectGUID de volta ao atributo msDS-ConsistencyGuid no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="15d29-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="15d29-108">Depois que o atributo msDS-ConsistencyGuid for preenchido, o Azure AD Connect exportará o objeto para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="15d29-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="15d29-109">**Observação:** Depois que um objeto AD local é importado para o Azure AD Connect (ou seja, importado para o Espaço do Conector do AD e projetado para o Metaverso), você não pode mais alterar seu valor sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="15d29-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="15d29-110">Para especificar o valor sourceAnchor para um determinado objeto AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="15d29-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="15d29-111">Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Connect: Conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="15d29-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

