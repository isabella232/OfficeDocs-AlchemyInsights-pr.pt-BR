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
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento consistencyGuid /sourceAnchor

O Azure AD Connect (versão 1.1.524.0 e depois) agora facilita o uso do msDS-ConsistencyGuid como atributo sourceAnchor. Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User. ObjectGUID é usado para outros tipos de objeto.
    
- Para qualquer determinado objeto usuário do AD local cujo atributo msDS-ConsistencyGuid não está preenchido, o Azure AD Connect grava seu valor objectGUID de volta ao atributo msDS-ConsistencyGuid no Active Directory local. Depois que o atributo msDS-ConsistencyGuid for preenchido, o Azure AD Connect exportará o objeto para o Azure AD.
    
 **Observação:** Depois que um objeto AD local é importado para o Azure AD Connect (ou seja, importado para o Espaço do Conector do AD e projetado para o Metaverso), você não pode mais alterar seu valor sourceAnchor. Para especificar o valor sourceAnchor para um determinado objeto AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Connect: Conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

