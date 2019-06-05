---
title: Adicionar um grupo a um site do SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719470"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Criar site conectado ao grupo no SharePoint Online

<p><strong>Há alguns problemas comuns encontrados durante a criação ou recriação de um site conectado ao grupo.&nbsp;</strong></p>  <p>1.Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.</p>  <ul>  <li>Baixe <a title="o Shell de gerenciamento do SpO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Shell</a> - de gerenciamento do SPO para obter mais informações sobre como começar a <a title="usar o PowerShell, confira introdução ao Shell de gerenciamento do SharePoint Online" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Introdução ao shell</a>de gerenciamento do SharePoint Online. <br /><br /></li>  <li>Remova o site de sites excluídos usando o <a title="remove-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-SPODeletedSite</a> cmdlet do PowerShell.</li>  </ul>  <p>Se você estiver criando um site conectado ao grupo e receber um aviso <strong>"outro grupo com o mesmo alias já existe"</strong>, verifique os grupos existentes do <a title="Office 365 no centro de administração" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 do centro</a>de administração. Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou crie o site com um alias diferente atribuído.&nbsp;</p>  <p><strong>Há diferentes maneiras de criar e usar grupos modernos com o SharePoint.&nbsp;</strong></p>  <ol>  <li>Você pode conectar sites existentes a um grupo do Office 365. Para obter mais informações, <a title="consulte Connect an Office 365 Group using the SharePoint User ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Conecte um grupo do Office 365 usando o usuário do</a>SharePoint ineterface.</li>  <li>Para criar um site conectado ao grupo do Office 365, você precisará criar um site de equipe. Para obter mais informações, <a title="consulte criar um site de equipe no SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Criar um site de equipe no SharePoint.</a></li>  </ol>

