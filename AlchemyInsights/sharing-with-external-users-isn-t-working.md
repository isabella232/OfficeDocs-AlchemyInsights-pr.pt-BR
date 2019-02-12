---
title: Compartilhando com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900852"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas ao compartilhar o conteúdo do SharePoint com usuários externos

Certifique-se de compartilhamento externo está ativado para a sua organização:
  
1. Vá até o [serviços &amp; página de suplementos no Centro de administração do Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.
    
2. Verifique se que a configuração está ativada para "Ligado". Se "Apenas usuários externos existentes" são selecionados, verifique se o usuário externo está listado no Centro de administração do Office 365.
    
Certifique-se de externo compartilhá-lo ativado para o site. Para um conjunto de sites clássico:
  
1. No Centro de administração do SharePoint clássico, no painel esquerdo, clique em **conjuntos de sites**.
    
2. Selecione o site ou sites e na faixa de opções, clique em **compartilhar**.
    
Para um site de equipe que pertence a um grupo do Office 365, ou um site de comunicação:
  
- Esses novos tipos de site têm o compartilhamento mesmo definindo como sua configuração de toda a organização, a menos que a configuração de toda a organização permite o compartilhamento de arquivos usando links que não exigem entrar. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que entram. Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint (preview) ou PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A configuração de compartilhamento externa para qualquer site pode ser mais restritiva do que a configuração de toda a organização, mas não mais permissivo do que a configuração de toda a organização. 
  

