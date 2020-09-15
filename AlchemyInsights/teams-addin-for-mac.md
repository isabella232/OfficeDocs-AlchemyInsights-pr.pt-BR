---
title: Complemento do Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670316"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="c3305-102">Complemento do Teams para Mac</span><span class="sxs-lookup"><span data-stu-id="c3305-102">Teams add-in for Mac</span></span>

<span data-ttu-id="c3305-103">Para solucionar os problemas de um complemento do Teams ausente para os usuários do sistema operacional Mac, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="c3305-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="c3305-104">**Passo 1:** se você tiver o Hybrid Exchange On Premises (2016 CU3 ou posterior necessário), utilize a ferramenta Test-HMA.ps1 para confirmar se a Autenticação Hybrid Modern está configurada corretamente.</span><span class="sxs-lookup"><span data-stu-id="c3305-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="c3305-105">Para mais informações, consulte [Validando a configuração da Autenticação Hybrid Modern para Outlook para iOS e Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="c3305-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="c3305-106">**Note** Use o formato de endereço UPN (por exemplo, [username@contoso.com](mailto:username@contoso.com)), não domínio\nome do usuário</span><span class="sxs-lookup"><span data-stu-id="c3305-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="c3305-107">Faça isso até mesmo para os usuários com caixas de correio no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c3305-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="c3305-108">**Passo 2:** Peça ao usuário que vá até **Ferramentas** > **Contas**... ,no Outlook para Mac, para encontrar e selecionar a conta.</span><span class="sxs-lookup"><span data-stu-id="c3305-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="c3305-109">Confirme se o nome do usuário listado está no formato UPN (por exemplo,, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="c3305-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="c3305-110">**Passo 3:** Confirme se o usuário possui uma licença do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c3305-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="c3305-111">O usuário deve estar utilizando a assinatura do Office 365 para Mac, versão 16.24 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c3305-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>