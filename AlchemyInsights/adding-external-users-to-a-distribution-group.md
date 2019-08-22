---
title: Adicionando usuários externos a um grupo de distribuição
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494515"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar usuários externos a um grupo de distribuição?

A adição de um contato externo a um grupo de distribuição (DG) é um processo de duas etapas:
  
1. Criar um contato de email para o usuário externo:
    
    1. No centro de administração, vá para a página[contatos](https://admin.microsoft.com/adminportal/home#/Contact) **dos usuários** > . 
    
    2. Selecione **Adicionar um contato**.
    
    3. Digite as informações do contato e selecione **Adicionar**.
    
2. Adicione o contato de email ao seu DG:
    
    1. No centro de administração, vá para a página grupos de **grupos** > [](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Localize o DG ao qual você deseja adicionar o usuário externo e selecione-o para abrir a caixa de diálogo Editar.
    
    3. Na guia **Membros** , selecione **Exibir todos e gerenciar Membros**. 
    
    4. Selecione **adicionar membros**.
    
    5. Selecione o contato de email que você criou na etapa anterior e, em seguida, selecione **salvar**.
    
Se após seguir estas etapas, seus usuários externos não podem enviar emails para o DG ou não receber emails dele, pode ser que o DG esteja marcado para permitir apenas emails de usuários internos. Você pode verificar essa configuração e corrigi-la seguindo as instruções [aqui](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Observação:** Essas instruções não se aplicam se o tipo de seu grupo for "Office 365 Group" em vez de "grupo de distribuição". Se esse for o caso, você poderá adicionar o usuário externo diretamente ao grupo do Outlook. Informações detalhadas sobre o Office 365 grupos convidados, bem como instruções para adicionar convidados externos, podem ser encontradas neste [artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  