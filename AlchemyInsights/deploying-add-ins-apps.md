---
title: Implantando os complementos para Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233501"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Implantando os complementos para Microsoft 365 Apps

A Implantação Centralizada é a maneira recomendada de implantar Office de usuários e grupos em sua organização. Para implantar os complementos, siga as etapas abaixo:

**Observação:** Para instalar os Office como um usuário individual, consulte Exibir, gerenciar e instalar os [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Além disso, certifique-se de que a aquisição individual de Office de complementos da Loja está habilitada. Para obter detalhes, consulte [Prevent add-in downloads by off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Verifique se seu ambiente atende aos requisitos de implantação de complementos usando a Implantação Centralizada. Para obter detalhes, consulte [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Vá para **Configurações**  >  **Aplicativos Integrados** Obter aplicativos no centro de administração  >   Microsoft 365 para implantar os complementos. 

Observações: 

- Os aplicativos integrados exigem que o administrador tenha permissões de Administrador Global ou Exchange Administrador.

- Ao implantar os complementos em vários usuários, recomendamos fazer atribuições usando grupos em vez de usuários individuais. Para obter detalhes, consulte Considerações ao atribuir um [complemento a usuários e grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- A Implantação Centralizada não dá suporte a usuários em grupos ou grupos aninhados que têm grupos pai. Para obter detalhes, consulte [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Verifique se o Microsoft 365 Serviço de Gerenciamento de Aplicativos (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') está habilitado para os usuários entrarem. Para obter detalhes, consulte [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Se você tiver problemas ao implantar os complementos usando Aplicativos Integrados, tente implantar usando [Os Complementos](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Para saber mais, veja:

[Implantar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gerenciar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Usar os cmdlets do PowerShell de Implantação Centralizada para gerenciar os complementos](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office-ins usando a Implantação Centralizada por meio do Microsoft 365 de administração](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Solução de problemas: o usuário não está](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) vendo os complementos 
 [Solucionar erros de usuário com Office Desem seguida](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)