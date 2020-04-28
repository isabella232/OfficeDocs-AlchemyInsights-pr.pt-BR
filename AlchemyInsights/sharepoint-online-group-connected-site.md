---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912954"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas durante a criação de um site conectado ao grupo no SharePoint

1. Alguns problemas comuns encontrados durante a criação ou recriação de um site conectado ao grupo.
Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.

   - Baixe o [Shell de gerenciamento do SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para obter mais informações sobre como começar a usar o PowerShell, confira [introdução ao Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Remova o site de sites excluídos usando o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) do PowerShell. O PowerShell é necessário para excluir permanentemente sites de grupo.

1. Se você estiver criando um site conectado ao grupo e receber um aviso: **outro grupo com o mesmo alias já existe**, verifique os grupos existentes no [centro de administração do Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou crie o site com um alias diferente atribuído.

1. Há diferentes maneiras de criar e usar grupos modernos com o SharePoint.

   - Você pode conectar sites existentes a um grupo do Microsoft 365. Para obter mais informações, consulte [Connect an Microsoft 365 Group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Para criar um site conectado ao grupo 365 da Microsoft, você precisará criar um [site de equipe](https://admin.microsoft.com/sharepoint).
