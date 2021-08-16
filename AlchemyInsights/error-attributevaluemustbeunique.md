---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002108"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é que dois objetos com SourceAnchor (immutableId) diferentes têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique o proxy duplicadoAddresses, userPrincipalName ou outro valor de atributo que está causando o erro. Identifique também quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Conexão Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual objeto deve continuar com o valor duplicado e qual objeto não deve.
    
3. Remova o valor duplicado do objeto que NÃO deve ter esse valor. Observe que você deve fazer a alteração no diretório de onde o objeto é origem. Em alguns casos, talvez seja necessário excluir um dos objetos em conflito.
    
4. Se você fez a alteração no AD local, deixe o Azure AD Conexão sincronizar a alteração para que o erro seja corrigido.
    

