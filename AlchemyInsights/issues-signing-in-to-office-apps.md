---
title: Problemas ao entrar em aplicativos do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833063"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="b7309-102">Corrigir os aplicativos do Microsoft 365 Mensagem "Desculpe, outra conta da sua organização já está assinada"</span><span class="sxs-lookup"><span data-stu-id="b7309-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="b7309-103">Para corrigir esse erro, use as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="b7309-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b7309-104">Remova todas as contas de trabalho, exceto a conta afetada, usando Configurações do Windows > **Trabalho ou escola do Access.**</span><span class="sxs-lookup"><span data-stu-id="b7309-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="b7309-105">[Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="b7309-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b7309-106">**Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="b7309-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b7309-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b7309-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b7309-108">Abra um aplicativo do Office, escolha **Sair** da  >  **Conta**  >  **de Arquivo**. Em seguida, entre usando uma conta de usuário com uma licença válida.</span><span class="sxs-lookup"><span data-stu-id="b7309-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="b7309-109">Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="b7309-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b7309-110">Para o Mac, consulte [Não é possível entrar em um aplicativo do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="b7309-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="b7309-111">Para obter mais informações, consulte ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="b7309-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>