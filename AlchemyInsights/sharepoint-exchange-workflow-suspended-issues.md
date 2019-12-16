---
title: Introdução ao SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051629"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="f9ae0-102">Workflows in SharePoint</span><span class="sxs-lookup"><span data-stu-id="f9ae0-102">Workflows in SharePoint</span></span>

<span data-ttu-id="f9ae0-103">Se os fluxos de trabalho do SharePoint não estiverem enviando emails, sua organização pode ter encontrado os limites de remetentes do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f9ae0-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="f9ae0-104">A mensagem de erro "o fluxo de trabalho é suspenso" pode ocorrer se você tiver um dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="f9ae0-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="f9ae0-105">Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="f9ae0-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="f9ae0-106">O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="f9ae0-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="f9ae0-107">Quando você executa o fluxo de trabalho, a mensagem de email não é enviada e você observa a mensagem de erro, o status interno é definido como suspenso ou não é possível enviar a um destinatário.</span><span class="sxs-lookup"><span data-stu-id="f9ae0-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="f9ae0-108">Para obter mais informações, consulte o [artigo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)a seguir.</span><span class="sxs-lookup"><span data-stu-id="f9ae0-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

