---
title: O compartilhamento com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369486"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de compartilhamento de conteúdo do SharePoint com usuários externos

Certifique-se de que o compartilhamento externo está ativado para sua organização:
  
1. Vá até a [página &amp; suplementos de serviços no centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **sites**.
    
2. Certifique-se de que a configuração está ativada para "ativado". Se "somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no centro de administração do Microsoft 365.
    
Verifique se o compartilhamento externo está ativado para o site. Para um conjunto de sites clássico:
  
1. No novo centro de administração do SharePoint, no painel esquerdo, clique em **sites**.
    
2. Selecione o site ou sites e, na faixa de opções, clique em **compartilhamento**.
    
Para um site de equipe que pertença a um grupo do Office 365 ou um site de comunicação:
  
- Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração em toda a organização, a menos que a configuração em toda a organização permita o compartilhamento de arquivos usando links que não exigem logon. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entram. Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização. 
  

