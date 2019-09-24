---
title: PowerShell do SharePoint Online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122987"
---
# <a name="sharepoint-online-powershell"></a>PowerShell do SharePoint Online

Trabalhar com o PowerShell ou scripts no SharePoint Online? Visite os links abaixo para obter mais informações.
- [Introdução ao Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Conectar-se ao PowerShell do SPO com a autenticação multifator (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Os [padrões e as práticas do SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contêm uma biblioteca de comandos do PowerShell que permite executar ações de gerenciamento complexas no SPO.

> [!NOTE]
> - Se você estiver tendo problemas para se conectar com o Shell de gerenciamento do SPO, verifique se você atualizou a versão mais recente e tente [reimportar o módulo](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) usando *"Import-Module Microsoft. online. SharePoint. PowerShell".*
> - Se você estiver tentando executar scripts de modelo de objeto do lado do cliente, será necessário ter o [SDK dos componentes do cliente do SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) instalado no computador local.
> - Se você estiver tendo problemas para executar scripts do PowerShell, convém considerar a execução do PowerShell como administrador e a alteração da [política de execução](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).