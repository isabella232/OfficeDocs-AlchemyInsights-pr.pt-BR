---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692753"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

Há várias maneiras de restringir o acesso aos serviços do SharePoint Online/OneDrive. Esses vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de permissão**

No SharePoint Online e no OneDrive for Business, restringe o acesso a itens como sites, arquivos e pastas concedendo acesso apenas aos grupos/pessoas que devem ter acesso.

- [Personalizar permissões para uma lista ou biblioteca do SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar as permissões de site do SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões em uma subpasta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não gerenciados](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um administrador do SharePoint ou global, você pode bloquear ou limitar o acesso ao conteúdo do SharePoint e do OneDrive de dispositivos não gerenciados (aqueles não associados ao AD híbrido ou em conformidade no Intune).

**Restrição de local de rede**

Como um administrador de ti, você pode controlar o acesso aos recursos do SharePoint e do OneDrive com base em locais de rede definidos nos quais confia. Isso também é conhecido como política baseada em local. Para obter mais informações, consulte [controlar o acesso aos dados do SharePoint Online e do onedrive com base no local da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de bloqueio de site** 

No SharePoint Online, você pode bloquear um conjunto de sites, portanto ninguém tem acesso. Isso é definido por meio do PowerShell e do [Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a propriedade [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Impedir que os usuários criem sites ou subsites**

Como administrador do SharePoint ou administrador global, você pode permitir que os usuários criem e administrem seus próprios sites do SharePoint, determine o tipo de sites que eles podem criar e especifique o local dos sites. Para obter mais informações, consulte [gerenciar a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

