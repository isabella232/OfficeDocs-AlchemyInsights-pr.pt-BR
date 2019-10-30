---
title: Solucionando problemas de mensagens de acesso negado para sites do OneDrive for Business
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766699"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Solucionando problemas de mensagens de acesso negado para sites do OneDrive for Business

Esse problema ocorre com mais frequência quando um usuário é excluído e recriado com o mesmo nome de usuário principal (UPN). A nova conta é criada usando um valor diferente de PUID (ID exclusiva do Passport). Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretório com uma unidade organizacional (OU) do Active Directory. Se os usuários já tiverem entrado no SharePoint e forem movidos para uma OU diferente e ressincronizado com o SharePoint, poderão enfrentar esse problema.

1. Para resolver esse problema, você deve restaurar o UPN original com as etapas no artigo, [restaurar um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Se não for possível restaurar o usuário original, remova o usuário antigo do site do OneDrive usando estas etapas, [remova um usuário da lista de informações do usuário](). 
3. Depois disso, você pode verificar se o usuário tem direitos de administrador para o site do OneDrive seguindo as etapas para [Adicionar o administrador do onedrive de um usuário](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Para obter mais informações sobre níveis de permissão, confira o artigo [noções básicas sobre níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
