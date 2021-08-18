---
title: Definir ClientAccessServerEnabled como True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320344"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Definir ClientAccessServerEnabled como True

Se você não puder abrir uma mensagem de email criptografada e, em vez disso, ver um **anexo rpmsg,** execute as seguintes etapas:

1. Conecte-se ao PowerShell do Exchange Online.

    **Observação**: para se conectar ao Exchange Online PowerShell, você deve entrar usando um administrador global ou Exchange de administrador.

   a. Abra Windows PowerShell e execute o seguinte comando:`$UserCredential = Get-Credential`
   b. Na caixa Windows PowerShell Caixa de diálogo **Solicitação de** Credencial, insira sua conta de trabalho ou estudante e senha, c. Clique em **OK**. 

2. Execute o seguinte comando para criar uma nova sessão:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Execute o seguinte comando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Execute `Get-IRMConfiguration` o comando.

4. Verifique a **configuração ClientAccessServerEnabled.** 

    a. Se **a configuração ClientAccessServerEnabled** estiver definida como **False**, execute o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Dica:** feche sempre a sessão do powershell com o seguinte comando: `Remove-PSSession $Session`

Para obter mais informações, [consulte Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

