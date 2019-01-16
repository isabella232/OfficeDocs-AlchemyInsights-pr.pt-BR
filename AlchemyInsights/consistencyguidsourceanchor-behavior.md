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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274490"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor comportamento

Conectar do Azure AD (versão 1.1.524.0 e depois) agora facilita o uso de msDS-ConsistencyGuid como sourceAnchor atributo. Ao usar esse recurso, o Azure Connect da AD configura automaticamente as regras de sincronização para:
  
- Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos de usuário. ObjectGUID é usada para outros tipos de objeto.
    
- Para qualquer dado AD outro usuário local do objeto cujo atributo msDS-ConsistencyGuid não é preenchidas, Azure gravações AD conectar seu valor objectGUID de volta para o atributo msDS-ConsistencyGuid no Active Directory no local. Depois que o atributo msDS-ConsistencyGuid é preenchido, Connect do Azure AD, em seguida, exporta o objeto para o Windows Azure AD.
    
 **Observação:** Uma vez um local objeto AD é importado para o Azure Connect do AD (isto é, importado para o espaço de conector AD e projetado no metaverso), você não pode alterar seu valor sourceAnchor mais. Para especificar o valor de sourceAnchor para um dado local AD do objeto, configure o atributo msDS-ConsistencyGuid antes que será importado para conectar do Azure AD. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Connect do Azure AD: conceitos de Design](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

