---
title: Restringir o acesso em SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093788"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso em SharePoint ou OneDrive

Há muitas maneiras de restringir o acesso aos serviços SharePoint Online/OneDrive Online. Esses vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de Permissão**

No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, arquivos e pastas, concedendo acesso apenas a esses grupos/indivíduos que devem ter acesso.

- [Personalizar permissões para uma SharePoint ou biblioteca](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar as permissões de site do SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões em uma subpasta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não gerenciados](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um SharePoint ou administrador global, você pode bloquear ou limitar o acesso ao conteúdo SharePoint e OneDrive de dispositivos não gerenciadas (aqueles que não são híbridos ingressados ou compatíveis com o AD no Intune).

**Restrição de Local de Rede**

Como administrador de TI, você pode controlar o acesso a recursos SharePoint e OneDrive com base em locais de rede definidos em que você confia. Isso também é conhecido como política baseada em locais. Para obter mais informações, consulte [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de Bloqueio de Site** 

No SharePoint Online, você tem a capacidade de bloquear um conjunto de sites, para que ninguém tenha acesso. Isso é definido por meio do PowerShell e do Shell de Gerenciamento [SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a [propriedade Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir usuários da criação de sites ou subsites**

Como administrador SharePoint ou administrador global, você pode permitir que seus usuários criem e administrem seus próprios sites de SharePoint, determinem que tipo de sites eles podem criar e especifiquem o local dos sites. Para obter mais informações, consulte [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

