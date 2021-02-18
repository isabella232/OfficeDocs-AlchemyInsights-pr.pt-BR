---
title: Seus usuários recebem emails mal-intencionados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291780"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="73074-102">Os seus usuários recebem emails mal-intencionados?</span><span class="sxs-lookup"><span data-stu-id="73074-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="73074-103">Agora você pode facilmente relatar para A Microsoft usando os [Envios de Administradores no Centro de Conformidade e Segurança](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="73074-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="73074-104">As mensagens enviadas em [envios do administrador](https://sip.protection.office.com/reportsubmission) são verificadas e os seguintes resultados são exibidos no menu desdobrável **detalhes**:</span><span class="sxs-lookup"><span data-stu-id="73074-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="73074-105">Se houve falha na autenticação do email do remetente no momento da entrega.</span><span class="sxs-lookup"><span data-stu-id="73074-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="73074-106">Informações sobre quaisquer acessos à política que possam ter afetado ou substituído o veredicto de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="73074-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="73074-107">Resultados de detonação atuais para ver se os URLs ou arquivos contidos na mensagem eram maliciosos ou não.</span><span class="sxs-lookup"><span data-stu-id="73074-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="73074-108">Feedback dos avaliadores</span><span class="sxs-lookup"><span data-stu-id="73074-108">Feedback from graders</span></span>

<span data-ttu-id="73074-109">Se uma substituição for encontrada, a nova varredura deve ser concluída em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="73074-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="73074-110">Se não houvesse problema na autenticação do email ou se a entrega não fosse afetada por uma modificação, o feedback dos avaliadores poderia levar até um dia.</span><span class="sxs-lookup"><span data-stu-id="73074-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="73074-111">Se você discordar do veredicto final em uma mensagem, URL ou arquivo (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para nova varredura.</span><span class="sxs-lookup"><span data-stu-id="73074-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="73074-112">As chances são altas de que o veredicto mude depois de enviar a mensagem novamente.</span><span class="sxs-lookup"><span data-stu-id="73074-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="73074-113">Enquanto isso, você pode remover e-mails maliciosos das caixas de entrada dos usuários, seguindo as instruções [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="73074-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="73074-114">Os clientes com Microsoft Defender para Office 365 podem:</span><span class="sxs-lookup"><span data-stu-id="73074-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="73074-115">use [Threat Explorer para Localizar e Excluir emails Suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="73074-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="73074-116">[use links seguros para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a um URL malicioso</span><span class="sxs-lookup"><span data-stu-id="73074-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="73074-117">rastrear usuários que clicaram e acessaram URLs maliciosos: [View URL de phishing e dados de veredicto de cliques](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="73074-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="73074-118">manualmente [iniciar uma Investigação Automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="73074-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="73074-119">Você também pode se proteger contra arquivos e URLs maliciosos, seguindo as instruções em [Proteção contra URLs e arquivos maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="73074-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>