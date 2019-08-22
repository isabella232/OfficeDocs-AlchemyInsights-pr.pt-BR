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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540889"
---
# <a name="how-to-disable-external-groups"></a>Como desabilitar grupos externos

A mensagem externa do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que as informações da empresa sejam compartilhadas. Para impedir que os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir o ETR a ser aplicado no Yammer:
  
- Faça logon no Yammer como um administrador verificado e, no **centro de administração do Yammer**, vá para **configurações de segurança \> de conteúdo e segurança** de C.

- Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online do Exchange (ETRs) no Yammer.**

- Escolha **Salvar**.

Para obter mais informações, consulte [controlar mensagens externas em uma rede do Yammer com regras de transporte do Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  