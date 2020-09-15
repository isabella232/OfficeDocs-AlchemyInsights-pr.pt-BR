---
title: Adicionando usuários externos a um grupo de distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663501"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar usuários externos a um grupo de distribuição

A adição de um contato externo a um grupo de distribuição (DG) é um processo de duas etapas:
  
1. Criar um contato de email para o usuário externo:
    
    1. No centro de administração, vá para a página contatos **dos usuários**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Selecione **Adicionar um contato**.
    
    3. Digite as informações do contato e selecione **Adicionar**.
    
2. Adicione o contato de email ao seu DG:
    
    1. No centro de administração, vá para a página grupos de **grupos**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Localize o DG ao qual você deseja adicionar o usuário externo e selecione-o para abrir a caixa de diálogo Editar.
    
    3. Na guia **Membros** , selecione **Exibir todos e gerenciar Membros**. 
    
    4. Escolha **Adicionar membros**.
    
    5. Selecione o contato de email que você criou na etapa anterior e, em seguida, selecione **salvar**.
    
Se após seguir estas etapas, seus usuários externos não podem enviar emails para o DG ou não receber emails dele, pode ser que o DG esteja marcado para permitir apenas emails de usuários internos. Você pode verificar essa configuração e corrigi-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Observação:** Estas instruções não se aplicam se o tipo de seu grupo for "Microsoft 365 Group" em vez de "grupo de distribuição". Se esse for o caso, você poderá adicionar o usuário externo diretamente ao grupo do Outlook. Informações detalhadas sobre os convidados de grupos do Microsoft 365, bem como instruções para a adição de convidados externos, podem ser encontradas neste [artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  