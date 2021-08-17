---
title: Solucionar problemas de mensagens negadas do Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085216"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Solucionar problemas de acesso mensagens negadas no Sharepoint/OneDrive Admin Center

Se você estiver recebendo uma mensagem de acesso negado ao tentar navegar até um Centro de Administração do Sharepoint/OneDrive, certifique-se de atribuir uma licença [ao usuário](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Se o usuário tiver uma licença, você [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) também deverá garantir que ele tenha uma função de administrador que possa acessar os centros de administração.

Esse problema também pode ocorrer quando um usuário é excluído e re-criado com o mesmo nome de entidade de usuário (UPN). A nova conta é criada usando um valor puid diferente (ID exclusiva do Passport). Quando o usuário tenta acessar um conjunto de sites ou suas OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (UO). Se os usuários já entraram no SharePoint e, em seguida, são movidos para uma OU diferente e ressínciados com o SharePoint, eles podem ter esse problema.

Para resolver esse problema, você deve restaurar o UPN original com as etapas do artigo, Restaurar um usuário [em](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365 .

Observação: se um centro de administração OneDrive ou SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.  [Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).


