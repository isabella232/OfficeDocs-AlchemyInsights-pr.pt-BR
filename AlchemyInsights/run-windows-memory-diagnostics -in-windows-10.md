---
title: Executar o diagnóstico de memória do Windows no Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720778"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="fcc34-102">Executar o diagnóstico de memória do Windows no Windows 10</span><span class="sxs-lookup"><span data-stu-id="fcc34-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="fcc34-103">Se o Windows e aplicativos em seu PC estiverem travando, congelando ou agindo de maneira instável, você poderá ter um problema com a memória (RAM) do PC.</span><span class="sxs-lookup"><span data-stu-id="fcc34-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="fcc34-104">Você pode executar o diagnóstico de memória do Windows para verificar se há problemas com a RAM do PC.</span><span class="sxs-lookup"><span data-stu-id="fcc34-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="fcc34-105">Na caixa de pesquisa na barra de tarefas, digite **diagnóstico de memória** e, em seguida, selecione **Diagnóstico de Memória do Windows**.</span><span class="sxs-lookup"><span data-stu-id="fcc34-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="fcc34-106">Para executar o diagnóstico, é necessário reiniciar o PC.</span><span class="sxs-lookup"><span data-stu-id="fcc34-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="fcc34-107">Você tem a opção de reiniciar imediatamente (salve o seu trabalho, feche os documentos e os emails abertos primeiro) ou agende o diagnóstico para ser executado automaticamente da próxima vez que o computador for reiniciado:</span><span class="sxs-lookup"><span data-stu-id="fcc34-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnóstico de Memória do Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="fcc34-109">Quando o computador for reiniciado, o **Ferramenta de Diagnóstico de Memória do Windows** será executado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="fcc34-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="fcc34-110">O status e o progresso serão exibidos como a execução do diagnóstico, e você terá a opção de cancelar o diagnóstico, pressionando a tecla **ESC** no teclado.</span><span class="sxs-lookup"><span data-stu-id="fcc34-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="fcc34-111">Quando o diagnóstico for concluído, o Windows será iniciado normalmente.</span><span class="sxs-lookup"><span data-stu-id="fcc34-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="fcc34-112">Imediatamente após a reinicialização, quando a área de trabalho for exibida, uma notificação aparecerá (ao lado do ícone **Central de Ações** na barra de tarefas) para indicar se foram encontrados erros de memória.</span><span class="sxs-lookup"><span data-stu-id="fcc34-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="fcc34-113">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fcc34-113">For example:</span></span>

<span data-ttu-id="fcc34-114">Este é o ícone da Central de Ações:</span><span class="sxs-lookup"><span data-stu-id="fcc34-114">Here's the Action Center icon:</span></span> ![Ícone da Central de Ações](media/action-center-icon.png) 

<span data-ttu-id="fcc34-116">E um exemplo de notificação:</span><span class="sxs-lookup"><span data-stu-id="fcc34-116">And a sample notification:</span></span> ![Nenhum erro de memória](media/no-memory-errors.png)

<span data-ttu-id="fcc34-118">Caso tenha perdido a notificação, você pode selecionar o ícone da **Central de Ações** na barra de tarefas para exibir a **Central de Ações** e ver uma lista rolável de notificações.</span><span class="sxs-lookup"><span data-stu-id="fcc34-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="fcc34-119">Para revisar informações detalhadas, digite **evento** na caixa de pesquisa na barra de tarefas e, em seguida, selecione **Visualizar Eventos**.</span><span class="sxs-lookup"><span data-stu-id="fcc34-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="fcc34-120">No painel esquerdo do **Visualizador de Eventos**, navegue até **Logs do Windows > Sistema**.</span><span class="sxs-lookup"><span data-stu-id="fcc34-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="fcc34-121">No painel à direita, examine a lista olhando para a coluna **Fonte**, até que você veja os eventos com o Valor da fonte **MemoryDiagnostics-Resultados**.</span><span class="sxs-lookup"><span data-stu-id="fcc34-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="fcc34-122">Realce cada evento e veja as informações de resultado na caixa abaixo da guia **Geral** da lista.</span><span class="sxs-lookup"><span data-stu-id="fcc34-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
