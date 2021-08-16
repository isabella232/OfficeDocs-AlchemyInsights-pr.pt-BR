---
title: Email de fluxo de trabalho não está sendo enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072508"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>O email do fluxo de trabalho não está sendo enviado para uma SharePoint ou biblioteca

1. Emails de fluxos de trabalho não são enviados para todos os usuários ou somente usuários específicos, ou você vê o erro A mensagem de email não pode ser **enviada. Certifique-se** de que o email tenha um destinatário válido.

    Verifique se o usuário existe no grupo **Todas as Pessoas** permissões (lista de informações do usuário) para esse conjunto de sites.  Url direta de exemplo: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Se o usuário não existir, certifique-se de que o usuário está entrando na página. 
    - Se for um usuário externo, certifique-se de que o convite foi aceito.
    - Se o usuário existir no grupo de permissões, certifique-se de que o endereço de email está correto.
    - Se o endereço de email dos usuários não estiver definido aqui, crie um alerta de exemplo para esse usuário que força a sincronização dessa conta de usuário dos Perfis de Usuário SharePoint para esse conjunto de sites.
 
2. Os emails de fluxos de trabalho são enviados para os administradores do conjunto de sites, mas não para outros usuários e veem o erro HTTP Proibido para **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Consulte [Acesso Negado ao enviar um email para um SharePoint grupo](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Além disso, verifique se **o** recurso de conjunto de sites do modo de bloqueio de permissão de usuário de acesso limitado não está ativo.


## <a name="related-topics"></a>Tópicos relacionados
Quer tentar Microsoft Flow no SharePoint Online?
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


