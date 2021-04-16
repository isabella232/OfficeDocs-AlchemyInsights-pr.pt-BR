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
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erro: as regras neste computador não corresponderão

Para ver o status atualizado desse problema conhecido, consulte As regras neste computador não combinam [com as regras no Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

A Equipe do Outlook implementou uma correção no Build 12928.10000. A correção já está no Insider Fast e irá para o Canal Mensal no final de junho de 2020. Depois de ter a com build fixa, você pode obter o prompt "Quais regras você deseja manter" uma última vez. Escolha Servidor quando solicitado e volte para o Outlook e habilita todas as regras que foram desabilitadas.

Até a correção estar disponível, use a seguinte solução alternativa:

**Solução alternativa**: em relatórios recentes, o problema ocorreu para aqueles que criaram apenas regras de cliente na área de trabalho do Outlook. Se você continuar a executar o problema, considere excluir as regras e, em seguida, criar e editar regras somente no OWA (Outlook Web App) até que o problema seja resolvido.

Se você não puder excluir as regras manualmente, poderá executar um comando do Outlook ao iniciar o Outlook executando Outlook.exe /cleanrules. Isso excluirá as regras de cliente e servidor. Ele excluirá todas as regras de todas as contas no Perfil do Outlook. Este comando é documentado ainda mais no artigo Opções de linha de comando.

