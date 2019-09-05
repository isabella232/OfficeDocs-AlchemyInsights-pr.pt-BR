---
title: Solucionar problemas de mensagens de acesso negado
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751264"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Solucionar problemas de mensagens de acesso negado no centro de administração do SharePoint/OneDrive

Se você estiver recebendo uma mensagem de acesso negado ao tentar navegar até um centro de administração do SharePoint/OneDrive, certifique-se de [atribuir uma licença ao usuário](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Se o usuário tiver uma licença, você também deve certificar-se de que ela é [atribuída a uma função de administrador](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) que pode acessar os centros de administração.

Esse problema também pode ocorrer quando um usuário é excluído e recriado com o mesmo nome de usuário principal (UPN). A nova conta é criada usando um valor diferente de PUID (ID exclusiva do Passport). Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretório com uma unidade organizacional (OU) do Active Directory. Se os usuários já tiverem entrado no SharePoint e forem movidos para uma OU diferente e ressincronizado com o SharePoint, poderão enfrentar esse problema.

Para resolver esse problema, você deve restaurar o UPN original com as etapas no artigo, [restaurar um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Observação: se um centro de administração do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.  [Verifique o painel de integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).


