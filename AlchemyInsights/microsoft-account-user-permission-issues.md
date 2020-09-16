---
title: Problema de solução de problemas-usuário não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725395"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problema de solução de problemas-usuário não encontrado no diretório

Se os usuários estiverem recebendo a mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o tipo de problema não é usuário no diretório.

As etapas a seguir podem ser concluídas para solucionar o problema.

- Verifique se a conta que aceitou o convite por email é a mesma conta que está sendo usada para entrar mais tarde. Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site. 

Para obter mais informações, consulte [como gerenciar aliases para sua conta da Microsoft </a> para gerenciar o logon do Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue até cada (s) site (s) em que o usuário está recebendo o erro. 

Adicione "/_layouts/15/People.aspx/MembershipGroupId = 0" (dentro das aspas duplas) ao final da URL do site. 

Exemplo: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o usuário na lista.

- Clique em **remover permissões do usuário** da faixa de opções. 
-  Adicione novamente o usuário e reenvie o convite para o usuário.

