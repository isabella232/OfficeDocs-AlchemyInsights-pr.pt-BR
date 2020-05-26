---
title: Precisa marcar um remetente de domínio ou e-mail como seguro?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281115"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="159da-102">Precisa marcar um remetente de domínio ou e-mail como seguro?</span><span class="sxs-lookup"><span data-stu-id="159da-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="159da-103">O uso de **listas de remetentes seguros não é recomendado**, pois abre sua organização a ataques de spam, phishing e falsificação.</span><span class="sxs-lookup"><span data-stu-id="159da-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="159da-104">No entanto, se houver uma necessidade comercial, **recomendamos** usar **[Regras de fluxo de e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para isso.</span><span class="sxs-lookup"><span data-stu-id="159da-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="159da-105">Nossa orientação garante a autenticação do remetente (verifica se o domínio de envio não está sendo falsificado).</span><span class="sxs-lookup"><span data-stu-id="159da-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="159da-106">**Observação**: não recomendamos o gerenciamento de falsos positivos usando listas de remetentes seguros, pois exceções à filtragem de spam podem abrir sua organização a ataques de segurança.</span><span class="sxs-lookup"><span data-stu-id="159da-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="159da-107">Se seus usuários receberem mensagens marcadas incorretamente como spam ou lixo eletrônico, **[Relate as mensagens e arquivos à Microsoft.](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="159da-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="159da-108">Remetentes seguros no Outlook, lista de remetentes permitidos ou lista de domínios permitidos nas políticas anti-spam **devem ser evitados** porque os remetentes ignoram toda a proteção contra spam, spoof e phishing e autenticação de remetente (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="159da-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="159da-109">Esse método é melhor usado apenas para testes temporários.</span><span class="sxs-lookup"><span data-stu-id="159da-109">This method is best used for temporary testing only.</span></span>
