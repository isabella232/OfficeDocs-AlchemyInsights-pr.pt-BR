---
title: Problema de solução de problemas-usuário não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702726"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problema de solução de problemas-usuário não encontrado no diretório

Se os usuários estiverem recebendo a mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o tipo de problema não é usuário no diretório.

As etapas a seguir podem ser concluídas para solucionar o problema.

- Verifique se a conta que aceitou o convite por email é a mesma conta que está sendo usada para entrar mais tarde. Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site. 

Para obter mais informações, consulte [como gerenciar aliases para sua conta</a> da Microsoft para gerenciar o logon do Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue até cada (s) site (s) em que o usuário está recebendo o erro. 

Adicione "/_layouts/15/People.aspx/MembershipGroupId = 0" (dentro das aspas duplas) ao final da URL do site. 

Exemplo: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o usuário na lista.

- Clique em **remover permissões do usuário** da faixa de opções. 
-  Adicione novamente o usuário e reenvie o convite para o usuário.

