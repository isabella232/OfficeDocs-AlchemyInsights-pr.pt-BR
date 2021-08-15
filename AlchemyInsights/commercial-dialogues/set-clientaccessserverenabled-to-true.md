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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994853"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Definir ClientAccessServerEnabled como True

Se você não puder abrir uma mensagem de email criptografada e, em vez disso, ver um **anexo rpmsg,** execute as seguintes etapas:

1. Conecte-se ao PowerShell do Exchange Online.

> [!NOTE]
> Para se conectar ao Exchange Online PowerShell, você deve entrar usando um administrador global ou Exchange conta de administrador.

   a. Abra Windows PowerShell e execute o seguinte comando:`$UserCredential = Get-Credential`
b. Na caixa Windows PowerShell Caixa de diálogo **Solicitação de** Credencial, insira sua conta de trabalho ou estudante e senha, c. Clique em **OK**. 

2. Execute o seguinte comando para criar uma nova sessão:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Execute o seguinte comando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Execute `Get-IRMConfiguration` o comando.

4. Verifique a **configuração ClientAccessServerEnabled.** 

    a. Se **a configuração ClientAccessServerEnabled** estiver definida como **False**, execute o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Feche sempre a sessão do powershell com o seguinte comando: `Remove-PSSession $Session`

Para obter mais informações, [consulte Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

