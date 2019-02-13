---
title: Acesso condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935916"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com Intune

Usando o **Access condicional** com Intune exige 3 etapas: 
  
- Crie uma **Política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidos para acessar esses recursos. Por exemplo, um dispositivo deve ser compatível com antes de acessar o email corporativo. 
    
- Crie uma **Política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo é considerado compatível. Por exemplo, um dispositivo deve ter um pin de pelo menos 6 dígitos antes que ela é considerada compatível. 
    
- Garantindo a **Políticas de conformidade** e de **Políticas de acesso condicional** são destinadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Windows Azure Active Directory. 
    
Leia mais:
  
- [Práticas recomendadas de acesso condicionais](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introdução ao Access condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

