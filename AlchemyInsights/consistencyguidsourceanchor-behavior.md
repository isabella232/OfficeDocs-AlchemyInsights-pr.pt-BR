---
title: Comportamento ConsistencyGuid/atributo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516957"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento ConsistencyGuid/atributo

O Azure AD Connect (versão 1.1.524.0 e posterior) agora facilita o uso do atributo msDS-ConsistencyGuid as atributo. Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Use msDS-ConsistencyGuid como o atributo atributo para objetos de usuário. ObjectGUID é usado para outros tipos de objeto.
    
- Para qualquer objeto de usuário do AD local específico cujo atributo msDS-ConsistencyGuid não esteja preenchido, o Azure AD Connect grava seu valor objectGUID de volta para o atributo msDS-ConsistencyGuid no Active Directory local. Após o atributo msDS-ConsistencyGuid ser preenchido, o Azure AD Connect, exporta o objeto para o Azure AD.
    
 **Observação:** Depois que um objeto do AD local é importado para o Azure AD Connect (ou seja, importado para o espaço do conector do AD e projetado para o metaverso), você não pode mais alterar o valor de atributo. Para especificar o valor de atributo para um determinado objeto AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect. 
  
Para obter mais informações sobre o atributo e o ConsistencyGuid, consulte o seguinte: [Azure ad Connect: design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

