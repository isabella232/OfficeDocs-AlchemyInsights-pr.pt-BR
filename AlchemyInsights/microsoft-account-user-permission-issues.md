---
title: Problema de solução de problemas-usuário não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054798"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="54352-102">Problema de solução de problemas-usuário não encontrado no diretório</span><span class="sxs-lookup"><span data-stu-id="54352-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="54352-103">Se os usuários estiverem recebendo a mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o tipo de problema não é usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="54352-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="54352-104">As etapas a seguir podem ser concluídas para solucionar o problema.</span><span class="sxs-lookup"><span data-stu-id="54352-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="54352-105">Verifique se a conta que aceitou o convite por email é a mesma conta que está sendo usada para entrar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="54352-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="54352-106">Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site.</span><span class="sxs-lookup"><span data-stu-id="54352-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="54352-107">Para obter mais informações, consulte [como gerenciar aliases para sua conta</a> da Microsoft para gerenciar o logon do Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="54352-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="54352-108">Navegue até cada (s) site (s) em que o usuário está recebendo o erro.</span><span class="sxs-lookup"><span data-stu-id="54352-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="54352-109">Adicione "/_layouts/15/People.aspx/MembershipGroupId = 0" (dentro das aspas duplas) ao final da URL do site.</span><span class="sxs-lookup"><span data-stu-id="54352-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="54352-110">Exemplo: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="54352-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="54352-111">Selecione o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="54352-111">Select the user from the list.</span></span>

- <span data-ttu-id="54352-112">Clique em **remover permissões do usuário** da faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="54352-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="54352-113">Adicione novamente o usuário e reenvie o convite para o usuário.</span><span class="sxs-lookup"><span data-stu-id="54352-113">Add back the User and Resend the invite to the user.</span></span>

