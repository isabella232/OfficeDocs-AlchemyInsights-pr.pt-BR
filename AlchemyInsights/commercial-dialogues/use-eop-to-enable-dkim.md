---
title: Use Exchange Online PowerShell para habilitar o DKIM para um domínio específico
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070277"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Use Exchange Online PowerShell para habilitar o DKIM para um domínio específico

Se você não puder criar os registros DNS DKIM no centro de administração, tente usar Exchange Online PowerShell. 

Para criar um registro DNS DKIM usando Exchange Online PowerShell, execute as seguintes etapas:

1. Abra Windows PowerShell como administrador e execute os seguintes comandos na sequência descrita:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Se você tiver problemas para se conectar ao Exchange Online PowerShell, consulte [Conexão para Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Depois que você estiver conectado ao Exchange Online PowerShell, execute o seguinte comando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Depois que o comando acima tiver sido executado com êxito, execute o seguinte comando para encerrar Exchange Online sessão do PowerShell:

    `Remove-PSSession $Session` 



