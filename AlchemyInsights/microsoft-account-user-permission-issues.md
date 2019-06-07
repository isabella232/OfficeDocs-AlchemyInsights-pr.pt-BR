---
title: Criar e usar uma caixa de correio compartilhada
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762389"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="a1195-102">Problema de solução de problemas-usuário não encontrado no diretório</span><span class="sxs-lookup"><span data-stu-id="a1195-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="a1195-103">Se os usuários estão recebendo mensagem de erro "o usuário não pode ser encontrado" no diretório.</span><span class="sxs-lookup"><span data-stu-id="a1195-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="a1195-104">Tente novamente onde o tipo de problema não é usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="a1195-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="a1195-105">As etapas a seguir podem ser concluídas para solucionar o problema.</span><span class="sxs-lookup"><span data-stu-id="a1195-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="a1195-106">Verifique se a conta que aceitou o convite por email é a mesma conta que está sendo usada para entrar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="a1195-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="a1195-107">Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site.</span><span class="sxs-lookup"><span data-stu-id="a1195-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="a1195-108">Para obter mais informações, consulte [como gerenciar aliases para sua conta</a> da Microsoft para gerenciar o logon do Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="a1195-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="a1195-109">Navegue até cada (s) site (s) em que o usuário está recebendo o erro.</span><span class="sxs-lookup"><span data-stu-id="a1195-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="a1195-110">Adicione "/_layouts/15/People.aspx/MembershipGroupId = 0" (dentro das aspas duplas) ao final da URL do site.</span><span class="sxs-lookup"><span data-stu-id="a1195-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="a1195-111">Exemplo: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="a1195-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="a1195-112">Selecione o usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="a1195-112">Select the user from the list.</span></span>

- <span data-ttu-id="a1195-113">Clique em **remover permissões do usuário** da faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="a1195-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="a1195-114">Adicione novamente o usuário e reenvie o convite para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a1195-114">Add back the User and Resend the invite to the user.</span></span>

