---
title: Usar o PowerShell do Exchange Online para habilitar o DKIM para um domínio específico
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500603"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="07c6d-102">Usar o PowerShell do Exchange Online para habilitar o DKIM para um domínio específico</span><span class="sxs-lookup"><span data-stu-id="07c6d-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="07c6d-103">Se você não puder criar os registros DNS DKIM no centro de administração, tente usar o PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="07c6d-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="07c6d-104">Para criar um registro DNS DKIM usando o PowerShell do Exchange Online, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="07c6d-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="07c6d-105">Abra Windows PowerShell como administrador e execute os seguintes comandos na sequência descrita:</span><span class="sxs-lookup"><span data-stu-id="07c6d-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="07c6d-106">a.</span><span class="sxs-lookup"><span data-stu-id="07c6d-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="07c6d-107">b.</span><span class="sxs-lookup"><span data-stu-id="07c6d-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="07c6d-108">c.</span><span class="sxs-lookup"><span data-stu-id="07c6d-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="07c6d-109">Se você tiver problemas para se conectar ao PowerShell do Exchange Online, consulte [Conectar-se ao PowerShell do Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="07c6d-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="07c6d-110">Depois de se conectar ao PowerShell do Exchange Online, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="07c6d-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="07c6d-111">Depois que o comando acima tiver sido executado com êxito, execute o seguinte comando para encerrar a sessão do PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="07c6d-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



