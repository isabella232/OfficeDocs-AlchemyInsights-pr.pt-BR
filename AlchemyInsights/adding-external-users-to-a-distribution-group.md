---
title: Adicionar usuários externos a um grupo de distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934821"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar usuários externos a um grupo de distribuição

Adicionar um contato externo a um grupo de distribuição (DG) é um processo de duas etapas:
  
1. Crie um Contato de Email para o usuário externo:
    
    1. No centro de administração, vá para a **página Contatos**  >  [dos](https://admin.microsoft.com/adminportal/home#/Contact) Usuários. 
    
    2. Selecione **Adicionar um contato**.
    
    3. Digite as informações do seu contato e selecione **Adicionar**.
    
2. Adicione o Contato de Email ao seu DG:
    
    1. No centro de administração, vá para a página **Grupos**  >  [grupos.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Encontre o DG ao que você deseja adicionar o usuário externo e selecione-o para abrir a caixa de diálogo editar.
    
    3. Na guia **Membros,** selecione **Exibir todos e gerenciar membros**. 
    
    4. Escolha **Adicionar membros**.
    
    5. Selecione o Contato de Email criado na etapa anterior e selecione **Salvar**.
    
Se depois de seguir essas etapas, os usuários externos não puderem enviar emails para o DG ou não receberem emails dele, pode ser que o DG seja marcado para permitir apenas emails de usuários internos. Você pode verificar essa configuração e corrigi-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Observação:** Essas instruções não se aplicam se o tipo do grupo for "Microsoft 365 grupo" em vez de "Grupo de distribuição". Se esse for o caso, você poderá adicionar o usuário externo diretamente ao grupo de Outlook. Informações detalhadas sobre Microsoft 365 convidados de grupos, bem como instruções para adicionar convidados externos podem ser encontradas [neste artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  