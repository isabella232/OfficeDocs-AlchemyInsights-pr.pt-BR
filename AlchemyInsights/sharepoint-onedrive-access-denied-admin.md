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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707942"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Solucionar problemas de acesso mensagens negadas no Centro de Administração do Sharepoint/OneDrive

Se você estiver recebendo uma mensagem de acesso negado ao tentar navegar até um Centro de Administração do Sharepoint/OneDrive, certifique-se de atribuir uma licença [ao usuário](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Se o usuário tiver uma licença, você [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) também deverá garantir que ele tenha uma função de administrador que possa acessar os centros de administração.

Esse problema também pode ocorrer quando um usuário é excluído e re-criado com o mesmo nome de entidade de usuário (UPN). A nova conta é criada usando um valor puid diferente (ID exclusiva do Passport). Quando o usuário tenta acessar um conjunto de sites ou seu OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (UO). Se os usuários já entraram no SharePoint e, em seguida, são movidos para uma OU diferente e reanciados com o SharePoint, eles podem ter esse problema.

Para resolver esse problema, você deve restaurar o UPN original com as etapas do artigo, Restaurar um usuário [no Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Observação: se um Centro de Administração do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário.  [Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).


