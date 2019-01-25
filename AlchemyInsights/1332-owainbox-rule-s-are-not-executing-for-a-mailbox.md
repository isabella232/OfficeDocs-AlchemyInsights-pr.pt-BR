---
title: 1332 OWA - regra (s) de caixa de entrada é não executá-lo para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457515"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="72877-102">Uma regra de caixa de entrada não está funcionando conforme o esperado</span><span class="sxs-lookup"><span data-stu-id="72877-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="72877-103">Verifique se as configurações a seguir:</span><span class="sxs-lookup"><span data-stu-id="72877-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="72877-p101">Pode ser redirecionada uma mensagem encaminhada ou respondida para automaticamente com base nas regras de caixa de entrada apenas uma vez. Uma regra de redirecionar (uma regra de caixa de entrada ou uma regra de fluxo de email, também conhecido como uma regra de transporte) pode adicionar um máximo de destinatários de encaminhamento de dez a uma mensagem. Para obter mais informações, consulte [limites de regra de diário, transporte e a caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="72877-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="72877-p102">Regras de caixa de entrada não funcionam na caixa de correio de registro no diário alternativa. Para obter mais informações sobre a caixa de correio de registro no diário alternativa, consulte a [caixa de correio de registro no diário alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="72877-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="72877-109">Para corrigir esses problemas, consulte [2829319 KB](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="72877-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="72877-110">Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de caixa de entrada antes de escalonar o problema ao Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="72877-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="72877-111">Abra a caixa de correio no Outlook na web e clique em **configurações** \> **Opções** \> **Organizar email** \> **regras de caixa de entrada**.</span><span class="sxs-lookup"><span data-stu-id="72877-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="72877-112">Na parte inferior da página, clique em **se suas regras não estão funcionando clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="72877-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

