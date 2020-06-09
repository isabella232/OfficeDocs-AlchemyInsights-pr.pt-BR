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
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617955"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erro: as regras neste computador não correspondem

Para ver o status atualizado desse problema conhecido, confira [as regras deste computador não correspondem às regras no Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

A equipe do Outlook implementou uma correção no Build 12928,10000. A correção já está em um insider Fast e vai para o canal mensal no final de junho de 2020. Depois que você tiver a compilação fixa, poderá receber o prompt "quais regras você deseja manter" uma última vez. Escolha servidor quando solicitado e, em seguida, volte no Outlook e habilite novamente qualquer regra que tenha sido desabilitada.

Até que a correção esteja disponível, use a seguinte solução alternativa:

**Solução**: em relatórios recentes, o problema ocorreu para aqueles que têm apenas regras de cliente criadas na área de trabalho do Outlook. Se você continuar a executar o problema, considere excluir as regras e, em seguida, criar e editar regras somente no OWA (Outlook Web App) até que o problema seja resolvido.

Se não for possível excluir as regras manualmente, você poderá executar um comando do Outlook ao iniciar o Outlook executando o Outlook. exe/Cleanrules. Isso excluirá as regras de cliente e de servidor. Ele excluirá todas as regras para todas as contas no perfil do Outlook. Este comando está mais documentado no artigo de opções de linha de comando.