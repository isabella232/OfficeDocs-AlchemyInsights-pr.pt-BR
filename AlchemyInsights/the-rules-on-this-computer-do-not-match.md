---
title: 'Erro: as regras neste computador não correspondem'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664234"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="2bcdc-102">Erro: as regras neste computador não correspondem</span><span class="sxs-lookup"><span data-stu-id="2bcdc-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="2bcdc-103">Para ver o status atualizado desse problema conhecido, confira [as regras deste computador não correspondem às regras no Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="2bcdc-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="2bcdc-104">A equipe do Outlook implementou uma correção no Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="2bcdc-105">A correção já está em um insider Fast e vai para o canal mensal no final de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="2bcdc-106">Depois que você tiver a compilação fixa, poderá receber o prompt "quais regras você deseja manter" uma última vez.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="2bcdc-107">Escolha servidor quando solicitado e, em seguida, volte no Outlook e habilite novamente qualquer regra que tenha sido desabilitada.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="2bcdc-108">Até que a correção esteja disponível, use a seguinte solução alternativa:</span><span class="sxs-lookup"><span data-stu-id="2bcdc-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="2bcdc-109">**Solução**: em relatórios recentes, o problema ocorreu para aqueles que têm apenas regras de cliente criadas na área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="2bcdc-110">Se você continuar a executar o problema, considere excluir as regras e, em seguida, criar e editar regras somente no OWA (Outlook Web App) até que o problema seja resolvido.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="2bcdc-111">Se não for possível excluir as regras manualmente, você poderá executar um comando do Outlook ao iniciar o Outlook executando o Outlook. exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="2bcdc-112">Isso excluirá as regras de cliente e de servidor.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="2bcdc-113">Ele excluirá todas as regras para todas as contas no perfil do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="2bcdc-114">Este comando está mais documentado no artigo de opções de linha de comando.</span><span class="sxs-lookup"><span data-stu-id="2bcdc-114">This command is further documented in the Command-line switches article.</span></span>

