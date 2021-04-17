---
title: Configurar respostas automáticas para uma caixa de correio
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820922"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="dcf5b-102">Configurar respostas automáticas para uma caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="dcf5b-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="dcf5b-103">**Método 1**</span><span class="sxs-lookup"><span data-stu-id="dcf5b-103">**Method 1**</span></span>

1. <span data-ttu-id="dcf5b-104">Entre no portal do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dcf5b-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="dcf5b-105">Vá para **Usuários > Usuários ativos** (ou **Grupos > Caixas de correio compartilhadas** se você definir essa opção em uma caixa de correio compartilhada).</span><span class="sxs-lookup"><span data-stu-id="dcf5b-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="dcf5b-106">Selecione um usuário com uma caixa de correio do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcf5b-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="dcf5b-107">No menu do submenu à direita, vá para **Configurações de email > Respostas automáticas** (se for uma caixa de correio compartilhada, basta clicar **Respostas automáticas** no menu do submenu).</span><span class="sxs-lookup"><span data-stu-id="dcf5b-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="dcf5b-108">**Método 2**</span><span class="sxs-lookup"><span data-stu-id="dcf5b-108">**Method 2**</span></span>

1. <span data-ttu-id="dcf5b-109">Entre no portal de administração do Microsoft 365 usando as credenciais de administrador.</span><span class="sxs-lookup"><span data-stu-id="dcf5b-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="dcf5b-110">Escolha **Centros de Administração** e depois clique em **Exchange**. </span><span class="sxs-lookup"><span data-stu-id="dcf5b-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="dcf5b-111">Clique na imagem no canto superior direito, clique **Outro usuário** e, em seguida, selecione a caixa de correio de usuário que você deseja alterar.</span><span class="sxs-lookup"><span data-stu-id="dcf5b-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="dcf5b-112">No lado esquerdo, selecione **Opções**, clique em **Organizar email** e, em seguida, clique em **Respostas automáticas.**</span><span class="sxs-lookup"><span data-stu-id="dcf5b-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="dcf5b-113">**Método 3**</span><span class="sxs-lookup"><span data-stu-id="dcf5b-113">**Method 3**</span></span>

<span data-ttu-id="dcf5b-114">Execute os seguintes cmdlet no PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="dcf5b-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="dcf5b-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="dcf5b-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="dcf5b-116">Para obter mais informações sobre esse cmdlet, confira [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="dcf5b-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
