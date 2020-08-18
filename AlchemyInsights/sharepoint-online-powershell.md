---
title: PowerShell do SharePoint Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786877"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="a9246-102">PowerShell do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a9246-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="a9246-103">Trabalhar com o PowerShell ou scripts no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a9246-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="a9246-104">Visite os links abaixo para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a9246-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="a9246-105">Introdução ao Shell de Gerenciamento do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a9246-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="a9246-106">Conectar-se ao PowerShell do SPO com a autenticação multifator (MFA)</span><span class="sxs-lookup"><span data-stu-id="a9246-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="a9246-107">Os [padrões e as práticas do SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contêm uma biblioteca de comandos do PowerShell que permite executar ações de gerenciamento complexas no SPO.</span><span class="sxs-lookup"><span data-stu-id="a9246-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="a9246-108">Se você estiver tendo problemas para se conectar com o Shell de gerenciamento do SPO, verifique se você atualizou a versão mais recente e tente [reimportar o módulo](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) usando *"Import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="a9246-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="a9246-109">Se você estiver tentando executar scripts de modelo de objeto do lado do cliente, será necessário ter o [SDK dos componentes do cliente do SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) instalado no computador local.</span><span class="sxs-lookup"><span data-stu-id="a9246-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="a9246-110">Se você estiver tendo problemas para executar scripts do PowerShell, convém considerar a execução do PowerShell como administrador e a alteração da [política de execução](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="a9246-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>