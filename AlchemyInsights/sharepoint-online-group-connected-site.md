---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750508"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemas ao criar ou agrupar sites conectados no SharePoint Online

Há alguns problemas comuns encontrados durante a criação ou recriação de um site conectado ao grupo.

 Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.

Baixe o [Shell de gerenciamento do SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Para saber mais sobre como começar a usar o PowerShell, confira [introdução ao Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Remova o site de sites excluídos usando o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) do PowerShell.

Se você estiver criando um site conectado ao grupo e receber um aviso outro grupo com o mesmo alias já existe, verifique os grupos existentes do [Office 365 a partir do centro de administração](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou crie o site com um alias diferente atribuído.

Há diferentes maneiras de criar e usar grupos modernos com o SharePoint.

Você pode conectar sites existentes a um grupo do Office 365. Para obter mais informações, consulte [Connect an Office 365 Group using the SharePoint User ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Para criar um site conectado ao grupo do Office 365, você precisará criar um site de equipe. Para obter mais informações, consulte [criar um site de equipe no SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

