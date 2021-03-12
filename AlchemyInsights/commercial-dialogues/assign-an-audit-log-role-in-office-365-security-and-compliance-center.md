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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735396"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="9deec-102">Atribuir uma função de Log de Auditoria no Centro de Segurança e Conformidade do Office 365</span><span class="sxs-lookup"><span data-stu-id="9deec-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="9deec-103">Para pesquisar o log de auditoria do Office 365, um administrador deve ter a função **Logs de Auditoria Somente para Exibição** ou função **Logs de Auditoria** no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9deec-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="9deec-104">Essas funções são atribuídas aos grupos de funções Gerenciamento de Conformidade e Gerenciamento da Organização por padrão.</span><span class="sxs-lookup"><span data-stu-id="9deec-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="9deec-105">Os administradores globais no Office 365 e no Microsoft 365 são adicionados automaticamente como membros do grupo de função Gerenciamento da Organização.</span><span class="sxs-lookup"><span data-stu-id="9deec-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="9deec-106">Para permitir que um usuário pesquise com o nível mínimo de privilégios, crie um grupo de função personalizado no Exchange Online, adicione a função **Logs de Auditoria Somente para Exibição** ou função **Logs de Auditoria** e, em seguida, adicione o usuário como membro do novo grupo de função.</span><span class="sxs-lookup"><span data-stu-id="9deec-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="9deec-107">Para saber mais, confira [Gerenciar grupos de funções no Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e [Pesquise no log de auditoria no Centro de Conformidade e Segurança](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="9deec-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>