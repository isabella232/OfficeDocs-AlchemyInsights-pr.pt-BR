---
title: Erro AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709139"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é dois objetos com atributo diferentes (imutávelid) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique o proxyAddresses, userPrincipalName ou outro valor de atributo duplicado que está causando o erro. Também identifica quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique o objeto que deve continuar a ter o valor duplicado e o objeto não.
    
3. Remova o valor duplicado do objeto que não deve ter esse valor. Observe que você deve fazer a alteração no diretório de origem do objeto. Em alguns casos, talvez seja necessário excluir um dos objetos em conflito.
    
4. Se você fez a alteração no AD local, deixe que o Azure AD Connect sincronize a alteração para que o erro seja corrigido.
    

