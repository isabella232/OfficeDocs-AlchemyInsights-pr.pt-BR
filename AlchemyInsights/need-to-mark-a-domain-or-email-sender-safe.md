---
title: Precisa marcar um remetente de domínio ou e-mail como seguro?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792120"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="98e8c-102">Precisa marcar um remetente de domínio ou e-mail como seguro?</span><span class="sxs-lookup"><span data-stu-id="98e8c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="98e8c-103">O uso de **listas de remetentes seguros não é recomendado**, pois abre sua organização a ataques de spam, phishing e falsificação.</span><span class="sxs-lookup"><span data-stu-id="98e8c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="98e8c-104">No entanto, se houver uma necessidade comercial, **recomendamos** usar **[Regras de fluxo de e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para isso.</span><span class="sxs-lookup"><span data-stu-id="98e8c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="98e8c-105">Nossa orientação garante a autenticação do remetente (verifica se o domínio de envio não está sendo falsificado).</span><span class="sxs-lookup"><span data-stu-id="98e8c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="98e8c-106">**Observação**: não recomendamos o gerenciamento de falsos positivos usando listas de remetentes seguros, pois exceções à filtragem de spam podem abrir sua organização a ataques de segurança.</span><span class="sxs-lookup"><span data-stu-id="98e8c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="98e8c-107">Se seus usuários receberem mensagens marcadas incorretamente como spam ou lixo eletrônico, **[Relate as mensagens e arquivos à Microsoft.](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="98e8c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="98e8c-108">Remetentes seguros no Outlook, lista de remetentes permitidos ou lista de domínios permitidos nas políticas anti-spam **devem ser evitados** porque os remetentes ignoram toda a proteção contra spam, spoof e phishing e autenticação de remetente (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="98e8c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="98e8c-109">Esse método é melhor usado apenas para testes temporários.</span><span class="sxs-lookup"><span data-stu-id="98e8c-109">This method is best used for temporary testing only.</span></span>
