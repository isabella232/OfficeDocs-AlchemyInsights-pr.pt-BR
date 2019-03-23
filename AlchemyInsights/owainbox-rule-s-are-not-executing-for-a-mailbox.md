---
title: 1332 OWA-regra (s) de caixa de entrada não estão sendo executadas para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784330"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="7abe0-102">Uma regra de caixa de entrada não funciona como esperado</span><span class="sxs-lookup"><span data-stu-id="7abe0-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="7abe0-103">Verifique as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="7abe0-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="7abe0-104">Uma mensagem pode ser redirecionada, encaminhada ou respondida automaticamente com base nas regras de caixa de entrada apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="7abe0-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="7abe0-105">Uma regra de redirecionamento (uma regra de caixa de entrada ou regra de fluxo de emails, também conhecida como regra de transporte) pode adicionar no máximo dez destinatários de encaminhamento a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7abe0-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="7abe0-106">Para saber mais, confira [limites de regras de diário, transporte e caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="7abe0-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="7abe0-107">As regras de caixa de entrada não funcionam na caixa de correio de registro em diário alternativa.</span><span class="sxs-lookup"><span data-stu-id="7abe0-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="7abe0-108">Para obter mais informações sobre a caixa de correio de registro no diário alternativo, confira [caixa de correio de registro em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="7abe0-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="7abe0-109">Para corrigir esses problemas, confira [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="7abe0-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="7abe0-110">Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico da regra de caixa de entrada antes de escalonar o problema para o suporte da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="7abe0-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="7abe0-111">Abra a caixa de correio no Outlook na Web e clique em **Opções** \> de **configurações** \> organizar **regras de caixa de entrada**de **email** \> .</span><span class="sxs-lookup"><span data-stu-id="7abe0-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="7abe0-112">Na parte inferior da página, clique em **se suas regras não estiverem funcionando, clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="7abe0-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

