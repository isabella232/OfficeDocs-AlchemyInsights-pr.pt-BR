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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981101"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erro: as regras neste computador não corresponderão

Para ver o status atualizado deste problema conhecido, consulte As regras neste computador não corresponderão às regras [no Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

A Outlook Team implementou uma correção no Build 12928.10000. A correção já está no Insider Fast e irá para o Canal Mensal no final de junho de 2020. Depois de ter a com build fixa, você pode obter o prompt "Quais regras você deseja manter" uma última vez. Escolha Servidor quando solicitado e volte para Outlook e reabilitar todas as regras desabilitadas.

Até a correção estar disponível, use a seguinte solução alternativa:

**Solução alternativa**: Em relatórios recentes, o problema ocorreu para aqueles que criaram apenas regras de cliente Outlook área de trabalho. Se você continuar a executar o problema, considere excluir as regras e, em seguida, criar e editar regras somente no OWA (Outlook Web App) até que o problema seja resolvido.

Se você não puder excluir as regras manualmente, poderá executar um comando Outlook quando você iniciar Outlook executando Outlook.exe /cleanrules. Isso excluirá as regras de cliente e servidor. Ele excluirá todas as regras de todas as contas no Outlook Profile. Este comando é documentado ainda mais no artigo Opções de linha de comando.

