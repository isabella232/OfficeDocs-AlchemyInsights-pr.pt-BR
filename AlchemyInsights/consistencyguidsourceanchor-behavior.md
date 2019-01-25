---
title: ConsistencyGuid / sourceAnchor comportamento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498506"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="a722e-102">ConsistencyGuid / sourceAnchor comportamento</span><span class="sxs-lookup"><span data-stu-id="a722e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="a722e-p101">Conectar do Azure AD (versão 1.1.524.0 e depois) agora facilita o uso de msDS-ConsistencyGuid como sourceAnchor atributo. Ao usar esse recurso, o Azure Connect da AD configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="a722e-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="a722e-p102">Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos de usuário. ObjectGUID é usada para outros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="a722e-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="a722e-p103">Para qualquer dado AD outro usuário local do objeto cujo atributo msDS-ConsistencyGuid não é preenchidas, Azure gravações AD conectar seu valor objectGUID de volta para o atributo msDS-ConsistencyGuid no Active Directory no local. Depois que o atributo msDS-ConsistencyGuid é preenchido, Connect do Azure AD, em seguida, exporta o objeto para o Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a722e-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="a722e-p104">**Observação:** Uma vez um local objeto AD é importado para o Azure Connect do AD (isto é, importado para o espaço de conector AD e projetado no metaverso), você não pode alterar seu valor sourceAnchor mais. Para especificar o valor de sourceAnchor para um dado local AD do objeto, configure o atributo msDS-ConsistencyGuid antes que será importado para conectar do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a722e-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="a722e-111">Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Connect do Azure AD: conceitos de Design](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="a722e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

