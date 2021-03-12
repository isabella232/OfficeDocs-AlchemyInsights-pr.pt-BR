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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735412"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Usar o PowerShell do Exchange Online para habilitar o DKIM para um domínio específico

Se você não puder criar os registros DNS DKIM no centro de administração, tente usar o PowerShell do Exchange Online. 

Para criar um registro DNS DKIM usando o PowerShell do Exchange Online, execute as seguintes etapas:

1. Abra Windows PowerShell como administrador e execute os seguintes comandos na sequência descrita:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Se você tiver problemas para se conectar ao PowerShell do Exchange Online, consulte [Conectar-se ao PowerShell do Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Depois de se conectar ao PowerShell do Exchange Online, execute o seguinte comando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Depois que o comando acima tiver sido executado com êxito, execute o seguinte comando para encerrar a sessão do PowerShell do Exchange Online:

    `Remove-PSSession $Session` 



