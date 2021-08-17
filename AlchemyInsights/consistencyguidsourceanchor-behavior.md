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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044328"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento consistencyGuid /sourceAnchor

O Azure AD Conexão (versão 1.1.524.0 e depois) agora facilita o uso do msDS-ConsistencyGuid como atributo sourceAnchor. Ao usar esse recurso, o Azure AD Conexão configura automaticamente as regras de sincronização para:
  
- Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User. ObjectGUID é usado para outros tipos de objeto.
    
- Para qualquer objeto do Usuário do AD local cujo atributo msDS-ConsistencyGuid não é preenchido, o Azure AD Conexão grava seu valor objectGUID de volta ao atributo msDS-ConsistencyGuid no Active Directory local. Depois que o atributo msDS-ConsistencyGuid for preenchido, o Azure AD Conexão exportará o objeto para o Azure AD.
    
 **Observação:** Depois que um objeto AD local é importado para o Azure AD Conexão (ou seja, importado para o Espaço do Conector do AD e projetado para o Metaverso), você não pode mais alterar seu valor sourceAnchor. Para especificar o valor sourceAnchor para um determinado objeto AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Conexão. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Conexão: Conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

