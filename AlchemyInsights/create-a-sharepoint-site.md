---
title: Criar um site do SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080878"
---
# <a name="create-a-sharepoint-site"></a>Criar um site do SharePoint

Crie ou gerencie sites a partir [de Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ativos no SharePoint Admin Center. Para obter mais informações, consulte [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Dicas:

- Não **é** possível criar um site com a mesma URL de um site existente. Se você excluiu um site e deseja re-usar a URL, é possível que o site excluído ainda exista em [sites excluídos.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) O site precisará ser excluído permanentemente para re-usar a URL. Para remover completamente um site com o Powershell, consulte o exemplo de cmdlet [Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Alguns usuários podem não ser capazes de criar um site. [Consulte Gerenciar a criação de site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- É possível que o site apareça travado na criação **por mais** tempo do que o esperado. Se mais de 24 horas se passaram desde que você viu esse problema pela primeira vez, registre um tíquete de suporte. Em muitos casos, já estamos trabalhando em uma solução. Dê-nos pelo menos 24 horas para concluir uma solução.
