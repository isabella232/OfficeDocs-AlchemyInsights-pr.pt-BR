---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709058"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Trabalhando com o PowerShell ou scripts no Sharepoint Online? Visite os links abaixo para obter mais informações.
- [Introdução ao Shell de Gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Conectar-se ao PowerShell do SPO com a autenticação multifator (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [O SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contém uma biblioteca de comandos do PowerShell que permite executar ações de gerenciamento complexas em relação ao SPO.

> [!NOTE]
> - Se você estiver com problemas para se conectar ao shell de gerenciamento do SPO, certifique-se de ter atualizado para a versão mais recente e tente [importar](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) novamente o módulo usando *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Se você estiver tentando executar scripts de modelo de objeto do lado do cliente, precisará ter o [SDK](https://www.microsoft.com/download/details.aspx?id=42038) componentes do cliente do Sharepoint Online instalado em sua máquina local.
> - Se você estiver com problemas para executar scripts do PowerShell, considere a execução do PowerShell como administrador e a alteração da Política [de Execução.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)