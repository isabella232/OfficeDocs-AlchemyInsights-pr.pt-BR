---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720756"
---
# <a name="how-to-disable-external-groups"></a>Como desabilitar grupos externos

A mensagem externa do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que as informações da empresa sejam compartilhadas. Para impedir que os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir o ETR a ser aplicado no Yammer:
  
- Faça logon no Yammer como um administrador verificado e, no **centro de administração do Yammer**, vá para **configurações de segurança \> de conteúdo e segurança** de C.

- Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online do Exchange (ETRs) no Yammer.**

- Selecione **Salvar**.

Confira mais informações [em desabilitar mensagens externas em uma rede do Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  