---
title: Erro AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916512"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é dois objetos com diferente SourceAnchor (immutableId) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique o proxyAddresses duplicado, userPrincipalName ou outro valor do atributo que está causando o erro. Também identifica quais objetos duas (ou mais) estão envolvidos no conflito. O relatório gerado pelo Windows Azure AD conectar integridade para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual objeto deve continuar tenham o valor duplicado e qual objeto não deveria.
    
3. Remova o valor de duplicada do objeto que não deveria ter desse valor. Observe que você deve fazer a alteração no diretório onde o objeto é originado. Em alguns casos, talvez seja necessário excluir um dos objetos em conflito.
    
4. Se você fez a alteração do local no AD, permitem conectar do Azure AD sincronizar a alteração para o erro obter corrigido.
    

