---
title: Adicionar um grupo a um SharePoint site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318112"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas comuns ao criar um site conectado a um grupo no SharePoint

1. Se você tiver excluído um grupo e seu site conectado e quiser criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.

   - Baixar [o Shell de Gerenciamento de SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para obter mais informações sobre como começar a trabalhar com o Powershell, consulte [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Remova o Site de Sites Excluídos usando o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. O Powershell é necessário para excluir permanentemente sites de grupo.

1. Se você estiver criando um site conectado a um grupo e receber um aviso: outro grupo com o mesmo **alias** já existe , verifique os grupos existentes do Centro de administração do Microsoft 365 [.](https://admin.microsoft.com/AdminPortal/Home#/groups) Para resolver o problema, exclua o grupo existente se não for mais necessário ou crie o site com um alias diferente atribuído.

1. Há diferentes maneiras de criar e usar grupos modernos com SharePoint.

   - Você pode conectar sites existentes a um Microsoft 365 grupo. Para obter mais informações, [consulte Conexão um grupo Microsoft 365 usando a interface SharePoint usuário.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Para criar um Microsoft 365 de grupo conectado, você precisará criar um [Site de Equipe.](https://admin.microsoft.com/sharepoint)
