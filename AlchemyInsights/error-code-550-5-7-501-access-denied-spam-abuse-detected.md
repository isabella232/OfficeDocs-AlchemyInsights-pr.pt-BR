---
title: Código de erro 550 5.7.501 acesso negado, abuso de spam detectado
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36740129"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="d2cfd-102">550 5.7.501 acesso negado, abuso de spam detectado</span><span class="sxs-lookup"><span data-stu-id="d2cfd-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="d2cfd-103">Normalmente, essa mensagem ocorre quando os usuários enviam mensagens de email de endereços IP usando o domínio inicial *. onmicrosoft.com* atribuído a novos locatários no Office 365.</span><span class="sxs-lookup"><span data-stu-id="d2cfd-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="d2cfd-104">A maneira mais fácil de resolver esse problema é:</span><span class="sxs-lookup"><span data-stu-id="d2cfd-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="d2cfd-105">[Adicionar um domínio ao seu locatário](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="d2cfd-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="d2cfd-106">[Altere o endereço de email principal do usuário](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) para o novo domínio personalizado que você acabou de adicionar.</span><span class="sxs-lookup"><span data-stu-id="d2cfd-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
