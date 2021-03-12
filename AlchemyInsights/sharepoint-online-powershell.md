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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="a612c-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a612c-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="a612c-103">Trabalhando com o PowerShell ou scripts no Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="a612c-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="a612c-104">Visite os links abaixo para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a612c-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="a612c-105">Introdução ao Shell de Gerenciamento do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a612c-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="a612c-106">Conectar-se ao PowerShell do SPO com a autenticação multifator (MFA)</span><span class="sxs-lookup"><span data-stu-id="a612c-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="a612c-107">[O SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contém uma biblioteca de comandos do PowerShell que permite executar ações de gerenciamento complexas em relação ao SPO.</span><span class="sxs-lookup"><span data-stu-id="a612c-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="a612c-108">Se você estiver com problemas para se conectar ao shell de gerenciamento do SPO, certifique-se de ter atualizado para a versão mais recente e tente [importar](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) novamente o módulo usando *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="a612c-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="a612c-109">Se você estiver tentando executar scripts de modelo de objeto do lado do cliente, precisará ter o [SDK](https://www.microsoft.com/download/details.aspx?id=42038) componentes do cliente do Sharepoint Online instalado em sua máquina local.</span><span class="sxs-lookup"><span data-stu-id="a612c-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="a612c-110">Se você estiver com problemas para executar scripts do PowerShell, considere a execução do PowerShell como administrador e a alteração da Política [de Execução.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="a612c-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>