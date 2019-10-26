---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504982"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com o Intune

O uso do **acesso condicional** com o Intune requer três etapas: 
  
- Criar uma **política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos. Por exemplo, um dispositivo deve estar em conformidade antes de acessar o email corporativo. 
    
- Crie uma **política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade. 
    
- Garantir que as políticas de **conformidade** e **as políticas de acesso condicional** sejam direcionadas para os grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory. 
    
Leia mais:
  
- [Práticas recomendadas de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introdução ao acesso condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

