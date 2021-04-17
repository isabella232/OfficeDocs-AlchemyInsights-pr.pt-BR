---
title: Executar o diagnóstico de memória do Windows no Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826655"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Executar o diagnóstico de memória do Windows no Windows 10

Se o Windows e aplicativos em seu PC estiverem travando, congelando ou agindo de maneira instável, você poderá ter um problema com a memória (RAM) do PC. Você pode executar o diagnóstico de memória do Windows para verificar se há problemas com a RAM do PC.

Na caixa de pesquisa na barra de tarefas, digite **diagnóstico de memória** e, em seguida, selecione **Diagnóstico de Memória do Windows**. 

Para executar o diagnóstico, é necessário reiniciar o PC. Você tem a opção de reiniciar imediatamente (salve o seu trabalho, feche os documentos e os emails abertos primeiro) ou agende o diagnóstico para ser executado automaticamente da próxima vez que o computador for reiniciado:

![Diagnóstico de Memória do Windows](media/windows-memory-diagnostic.png)

Quando o computador for reiniciado, o **Ferramenta de Diagnóstico de Memória do Windows** será executado automaticamente. O status e o progresso serão exibidos como a execução do diagnóstico, e você terá a opção de cancelar o diagnóstico, pressionando a tecla **ESC** no teclado.

Quando o diagnóstico for concluído, o Windows será iniciado normalmente.
Imediatamente após a reinicialização, quando a área de trabalho for exibida, uma notificação aparecerá (ao lado do ícone **Central de Ações** na barra de tarefas) para indicar se foram encontrados erros de memória. Por exemplo:

Este é o ícone da Central de Ações: ![Ícone da Central de Ações](media/action-center-icon.png) 

E um exemplo de notificação: ![Nenhum erro de memória](media/no-memory-errors.png)

Caso tenha perdido a notificação, você pode selecionar o ícone da **Central de Ações** na barra de tarefas para exibir a **Central de Ações** e ver uma lista rolável de notificações.

Para revisar informações detalhadas, digite **evento** na caixa de pesquisa na barra de tarefas e, em seguida, selecione **Visualizar Eventos**. No painel esquerdo do **Visualizador de Eventos**, navegue até **Logs do Windows > Sistema**. No painel à direita, examine a lista olhando para a coluna **Fonte**, até que você veja os eventos com o Valor da fonte **MemoryDiagnostics-Resultados**. Realce cada evento e veja as informações de resultado na caixa abaixo da guia **Geral** da lista.
