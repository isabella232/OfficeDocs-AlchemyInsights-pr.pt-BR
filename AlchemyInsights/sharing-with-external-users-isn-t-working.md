---
title: O compartilhamento com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304357"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de compartilhamento SharePoint conteúdo com usuários externos

Certifique-se de que o compartilhamento externo está ligado para sua organização:
  
1. Vá para a [página &amp; de complementos de serviços](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)no Centro de administração do Microsoft 365 , e clique em **Sites**.
    
2. Certifique-se de que a configuração está virada para "Ligado". Se "Somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no Centro de administração do Microsoft 365.
    
Certifique-se de que o compartilhamento externo está ligado para o site. Para um conjunto de sites clássico:
  
1. No novo SharePoint de administração, no painel esquerdo, clique em **sites**.
    
2. Selecione o site ou sites e, na faixa de opções, clique em **Compartilhar**.
    
Para um site de equipe que pertence a um grupo Microsoft 365, ou a um site de comunicação:
  
- Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração de toda a organização, a menos que a configuração em toda a organização permita o compartilhamento de arquivos usando links que não exigem entrar. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entrarem. Para alterar a configuração de sites específicos, use o novo centro de administração SharePoint ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Observação**: a configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização. 
  

