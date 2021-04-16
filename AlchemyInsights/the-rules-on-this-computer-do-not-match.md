---
title: 'Erro: as regras neste computador não corresponderão'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782940"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="ae5d7-102">Erro: as regras neste computador não corresponderão</span><span class="sxs-lookup"><span data-stu-id="ae5d7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="ae5d7-103">Para ver o status atualizado desse problema conhecido, consulte As regras neste computador não combinam [com as regras no Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="ae5d7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="ae5d7-104">A Equipe do Outlook implementou uma correção no Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="ae5d7-105">A correção já está no Insider Fast e irá para o Canal Mensal no final de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="ae5d7-106">Depois de ter a com build fixa, você pode obter o prompt "Quais regras você deseja manter" uma última vez.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="ae5d7-107">Escolha Servidor quando solicitado e volte para o Outlook e habilita todas as regras que foram desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="ae5d7-108">Até a correção estar disponível, use a seguinte solução alternativa:</span><span class="sxs-lookup"><span data-stu-id="ae5d7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="ae5d7-109">**Solução alternativa**: em relatórios recentes, o problema ocorreu para aqueles que criaram apenas regras de cliente na área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="ae5d7-110">Se você continuar a executar o problema, considere excluir as regras e, em seguida, criar e editar regras somente no OWA (Outlook Web App) até que o problema seja resolvido.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="ae5d7-111">Se você não puder excluir as regras manualmente, poderá executar um comando do Outlook ao iniciar o Outlook executando Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="ae5d7-112">Isso excluirá as regras de cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="ae5d7-113">Ele excluirá todas as regras de todas as contas no Perfil do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="ae5d7-114">Este comando é documentado ainda mais no artigo Opções de linha de comando.</span><span class="sxs-lookup"><span data-stu-id="ae5d7-114">This command is further documented in the Command-line switches article.</span></span>

