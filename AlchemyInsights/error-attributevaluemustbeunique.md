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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766012"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é dois objetos com atributo diferentes (imutávelid) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique o proxyAddresses, userPrincipalName ou outro valor de atributo duplicado que está causando o erro. Também identifica quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique o objeto que deve continuar a ter o valor duplicado e o objeto não.
    
3. Remova o valor duplicado do objeto que não deve ter esse valor. Observe que você deve fazer a alteração no diretório de origem do objeto. Em alguns casos, talvez seja necessário excluir um dos objetos em conflito.
    
4. Se você fez a alteração no AD local, deixe que o Azure AD Connect sincronize a alteração para que o erro seja corrigido.
    

