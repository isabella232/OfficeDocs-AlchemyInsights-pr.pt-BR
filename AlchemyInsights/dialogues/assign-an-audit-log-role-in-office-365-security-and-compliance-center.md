---
title: Atribuir uma função de Log de Auditoria no Centro de Segurança e Conformidade do Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509501"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Atribuir uma função de Log de Auditoria no Centro de Segurança e Conformidade do Office 365

Para pesquisar o log de auditoria do Office 365, um administrador deve ter a função **Logs de Auditoria Somente para Exibição** ou função **Logs de Auditoria** no Exchange Online. Essas funções são atribuídas aos grupos de funções Gerenciamento de Conformidade e Gerenciamento da Organização por padrão. Os administradores globais no Office 365 e no Microsoft 365 são adicionados automaticamente como membros do grupo de função Gerenciamento da Organização.

Para permitir que um usuário pesquise com o nível mínimo de privilégios, crie um grupo de função personalizado no Exchange Online, adicione a função **Logs de Auditoria Somente para Exibição** ou função **Logs de Auditoria** e, em seguida, adicione o usuário como membro do novo grupo de função.

Para saber mais, confira [Gerenciar grupos de funções no Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e [Pesquise no log de auditoria no Centro de Conformidade e Segurança](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).