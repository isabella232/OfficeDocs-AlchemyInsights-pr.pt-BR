---
title: Solucionar problemas - Usuário não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098158"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Solucionar problemas - Usuário não encontrado no diretório

Se os usuários estão recebendo a mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o Tipo de Problema é Usuário não no diretório.

As etapas a seguir podem ser concluídas para solucionar o problema.

- Certifique-se de que a conta que aceitou o convite de email seja a mesma que está sendo usada para entrar mais tarde. Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site. 

Para obter mais informações, [consulte Como gerenciar aliases para sua conta da Microsoft </a> para gerenciar o Microsoft 365 logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue até cada(s) site(s) no qual o usuário está recebendo o erro. 

Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (entre aspas duplas) ao final da URL do site. 

Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o usuário na lista.

- Clique **em Remover Permissões do** Usuário da Faixa de Opções. 
-  Adicione novamente o Usuário e Resenda o convite ao usuário.

