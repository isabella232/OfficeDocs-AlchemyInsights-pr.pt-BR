---
title: O email do fluxo de trabalho não está sendo enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049361"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>O email do fluxo de trabalho não está sendo enviado para uma lista ou biblioteca do SharePoint

1. O email de fluxos de trabalho não é enviado a todos os usuários ou apenas usuários específicos, ou você vê o erro **a mensagem de email não pode ser enviada. Certifique-se de que o email tem um destinatário válido**.

    Verifique se o usuário existe no grupo de permissões **todas as pessoas** (lista de informações do usuário) para esse conjunto de sites.  URL direta de exemplo:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Se o usuário não existir, certifique-se de que o usuário está conectado à página. 
    - Se for um usuário externo, certifique-se de que seu convite tenha sido aceito.
    - Se o usuário existir no grupo permissões, certifique-se de que o endereço de email está correto.
    - Se o endereço de email dos usuários não estiver definido aqui, crie um alerta de exemplo para esse usuário que force a sincronização dessa conta de usuário dos perfis de usuário do SharePoint para este conjunto de sites.
 
2. Os emails de fluxos de trabalho são enviados para os administradores do conjunto de sites, mas não para outros usuários e confira o erro **http proibido para <span>https:</span>//URL/_vti_bin/Client.XVC.SP.Utilities.Utility.SendEmail**.
 

    Consulte [acesso negado ao enviar um email a um grupo do SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Além disso, verifique se o recurso de conjunto de sites do **modo de bloqueio de permissão de usuário de acesso limitado** não está ativo.


## <a name="related-topics"></a>Tópicos relacionados
Deseja experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e fluxo](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


