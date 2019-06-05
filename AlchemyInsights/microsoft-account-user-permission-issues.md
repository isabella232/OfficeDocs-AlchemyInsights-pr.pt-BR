---
title: Criar e usar uma caixa de correio compartilhada
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717335"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problema de solução de problemas-usuário não encontrado no diretório

<p>Se os usuários estiverem recebendo mensagem <strong> &ldquo; &hellip;de erro&rsquo;, o usuário não pode ser encontrado no diretório. Tente novamente&hellip; </strong> onde o tipo de problema não é <strong> &ldquo;usuário no diretório.&rdquo;</strong>, as etapas a seguir podem ser concluídas para solucionar o problema.</p> <ol> <li>Verifique se a conta que aceitou o convite por email é a mesma conta que está sendo usada para entrar mais tarde. Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site. <br /><br />Para obter mais informações, consulte <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">como gerenciar aliases para sua conta da Microsoft</a> para gerenciar o logon do Office 365. <br /><br /></li> <li>Navegue até cada (s) site (s) em que o usuário está recebendo o erro. <br /><br />a. Adicione <strong> &ldquo;/_layouts/15/People.aspx/MembershipGroupId = 0&rdquo; </strong> (dentro das aspas duplas) ao final da URL do site. <br /><br />Exemplo: https://&lt;contoso&gt;. SharePoint.com/_layouts/15/People.aspx/membershipGroupId=0 <br /><br />b. Selecione o usuário na lista. <br /><br />c. Clique em <strong>remover permissões do usuário da faixa de</strong>opções. <br /><br />d. Adicione novamente o usuário e reenvie o convite para o usuário.</li> </ol>

