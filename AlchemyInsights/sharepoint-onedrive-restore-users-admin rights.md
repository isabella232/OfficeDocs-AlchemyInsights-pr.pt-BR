---
title: Solução de problemas de mensagens negadas do Access para OneDrive for Business sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957781"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Solução de problemas de mensagens negadas do Access para OneDrive for Business sites

Esse problema ocorre com mais frequência quando um usuário é excluído e re-criado com o mesmo nome de entidade de usuário (UPN). A nova conta é criada usando um valor puid diferente (ID exclusiva do Passport). Quando o usuário tenta acessar um conjunto de sites ou suas OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (UO). Se os usuários já entraram no SharePoint e, em seguida, são movidos para uma OU diferente e ressínciados com o SharePoint, eles podem ter esse problema.

1. Para resolver esse problema, você deve restaurar o UPN original com as etapas do artigo, [Restaurar um usuário em](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365 .
2. Se você não puder restaurar o usuário original, remova o usuário antigo do site OneDrive usando essas etapas, Remova um usuário da lista de informações [do usuário](). 
3. Depois que isso for feito, você poderá verificar se o usuário tem [](https://docs.microsoft.com/sharepoint/manage-user-profiles) direitos de administrador no site OneDrive seguindo as etapas para Adicionar administradores para o OneDrive

Para obter mais informações sobre níveis de permissão, consulte o artigo, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
