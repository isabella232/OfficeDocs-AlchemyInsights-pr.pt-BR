---
title: Diversos usuários recebem o erro Acesso Negado ao adicionar suplementos ao Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065380"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Diversos usuários recebem o erro Acesso Negado ao adicionar suplementos ao Outlook

Você pode especificar quais administradores na sua organização têm permissão para instalar e gerenciar suplementos do Outlook. Você pode também especificar quais administradores na sua organização têm permissão para instalar e gerenciar suplementos para seu próprio uso.

Para obter mais detalhes, confira o artigo [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Para verificar se você conseguiu atribuir permissões a um usuário, substitua <Role Name> pelo nome da função a ser verificada e execute o seguinte comando no PowerShell do Exchange Online:

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

Esse exemplo mostra como verificar para quem você atribuiu permissões para instalar suplementos da Office Store na organização.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Nos resultados, Get-ManagementRoleAssignment, verifique as entradas na coluna Usuários Efetivos.

Para informações detalhadas de sintaxes e de parâmetros, consulte [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 