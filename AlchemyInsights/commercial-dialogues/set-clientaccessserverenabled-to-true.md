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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735431"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="a8e94-102">Definir ClientAccessServerEnabled como True</span><span class="sxs-lookup"><span data-stu-id="a8e94-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="a8e94-103">Se você não puder abrir uma mensagem de email criptografada e, em vez disso, ver um **anexo rpmsg,** execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="a8e94-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="a8e94-104">Conecte-se ao PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a8e94-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="a8e94-105">Para se conectar ao PowerShell do Exchange Online, você deve entrar usando um administrador global ou uma conta de administrador do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8e94-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="a8e94-106">a.</span><span class="sxs-lookup"><span data-stu-id="a8e94-106">a.</span></span> <span data-ttu-id="a8e94-107">Abra Windows PowerShell e execute o seguinte comando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="a8e94-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="a8e94-108">b.</span><span class="sxs-lookup"><span data-stu-id="a8e94-108">b.</span></span> <span data-ttu-id="a8e94-109">Na caixa Windows PowerShell caixa de diálogo **Solicitação de** Credencial, insira sua conta de trabalho ou estudante e senha, c.</span><span class="sxs-lookup"><span data-stu-id="a8e94-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="a8e94-110">Clique **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8e94-110">Click **OK**.</span></span> 

2. <span data-ttu-id="a8e94-111">Execute o seguinte comando para criar uma nova sessão:</span><span class="sxs-lookup"><span data-stu-id="a8e94-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="a8e94-112">a.</span><span class="sxs-lookup"><span data-stu-id="a8e94-112">a.</span></span> <span data-ttu-id="a8e94-113">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="a8e94-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="a8e94-114">Execute `Get-IRMConfiguration` o comando.</span><span class="sxs-lookup"><span data-stu-id="a8e94-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="a8e94-115">Verifique a **configuração ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="a8e94-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="a8e94-116">a.</span><span class="sxs-lookup"><span data-stu-id="a8e94-116">a.</span></span> <span data-ttu-id="a8e94-117">Se **a configuração ClientAccessServerEnabled** estiver definida como **False**, execute o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="a8e94-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="a8e94-118">Feche sempre a sessão do powershell com o seguinte comando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="a8e94-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="a8e94-119">Para obter mais informações, consulte [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="a8e94-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

