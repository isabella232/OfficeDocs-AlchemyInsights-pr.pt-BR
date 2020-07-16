---
title: O problema do spooler de impressão está resolvido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083918"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="7faaa-102">O problema do spooler de impressão está resolvido</span><span class="sxs-lookup"><span data-stu-id="7faaa-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="7faaa-103">Se o seu dispositivo foi atualizado com o Windows 10  **OS Build 19041.329**, você pode ter observado um problema onde algumas impressoras não estão conseguindo imprimir.</span><span class="sxs-lookup"><span data-stu-id="7faaa-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="7faaa-104">O spooler de impressão pode exibir um erro ou fechar inesperadamente ao tentar imprimir e não há qualquer saída a partir da impressora afetada.</span><span class="sxs-lookup"><span data-stu-id="7faaa-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="7faaa-105">Este problema está resolvido na versão **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="7faaa-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="7faaa-106">**Investigação em curso**</span><span class="sxs-lookup"><span data-stu-id="7faaa-106">**Ongoing investigation**</span></span>

<span data-ttu-id="7faaa-107">O arquivo do Serviço de Subsistema da Autoridade Local de Segurança (LSASS) (**Isass.exe**) pode falhar em alguns dispositivos e exibir a mensagem de erro, "Um processo crítico do sistema, C:\WINDOWS\system32\Isass.exe, falhou com o código de estatus c0000008.</span><span class="sxs-lookup"><span data-stu-id="7faaa-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="7faaa-108">O computador precisa ser reiniciado agora".</span><span class="sxs-lookup"><span data-stu-id="7faaa-108">The machine must now be restarted".</span></span>  <span data-ttu-id="7faaa-109">**A Microsoft está trabalhando na solução e vai fornecer uma atualização no próximo lançamento.**</span><span class="sxs-lookup"><span data-stu-id="7faaa-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="7faaa-110">Para obter mais informações, verifique os problemas conhecidos do [Windows 10 Versão 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="7faaa-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>