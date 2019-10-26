---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739481"
---
# <a name="how-to-disable-external-groups"></a>Como desabilitar grupos externos

A mensagem externa do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que as informações da empresa sejam compartilhadas. Para impedir que os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir o ETR a ser aplicado no Yammer:
  
- Faça logon no Yammer como um administrador verificado e, no **centro de administração do Yammer**, vá para **configurações de segurança \> de conteúdo e segurança** de C.

- Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online do Exchange (ETRs) no Yammer.**

- Escolha **Salvar**.

Confira mais informações [em desabilitar mensagens externas em uma rede do Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  