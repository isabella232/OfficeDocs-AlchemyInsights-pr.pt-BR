---
title: Alterar o domínio padrão do Yammer
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
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950104"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Alterar o domínio padrão/primário do Yammer

A URL do Yammer contém o nome de domínio primário atual da sua rede do Yammer. Talvez esse nome de domínio não corresponda ao nome de domínio primário definido no Office 365 ou no Azure AD. Há diferenças no comportamento de acordo com o número de domínios personalizados adicionados ao locatário e com a existência ou não de uma configuração compatível do Yammer (1 Locatário: 1 Rede ou 1:1). A documentação sobre [Domínios do Yammer e o Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) está disponível.

O motivo mais comum para você ver um domínio incorreto é a existência de várias redes do Yammer que precisam ser consolidadas. A [consolidação até uma única rede](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) usando a ferramenta de migração de rede é uma primeira etapa importante. Faça isso antes de tentar definir seu domínio primário.

**Domínios não personalizados**

Para novos locatários, o domínio padrão (por exemplo, fabrikam.onmicrosoft.com) do locatário será usado para o Yammer. O domínio primário é definido como yammer.com/fabrikam.onmicrosoft.com.

**Domínio único personalizado**

O Yammer selecionará automaticamente o domínio personalizado (por exemplo, fabrikam.com) do locatário como o domínio primário no Yammer. Ele foi definido como yammer.com/fabrikam.com. Essa alteração é feita pelo serviço de sincronização de domínio e pode demorar até 24 horas para entrar em vigor.

**Vários domínios personalizados**

O Yammer pode ter um domínio primário diferente do domínio do locatário padrão. Como há vários domínios personalizados, o Yammer não tenta adivinhar o domínio correto entre os disponíveis. É necessário abrir um caso de suporte para solicitar que o nome de domínio primário seja alterado para o domínio primário de sua escolha.

**Informações adicionais para solução de problemas**

Em alguns casos, talvez os domínios tenham sido movidos entre locatários, e o serviço de sincronização de domínio não conseguiu executar com êxito. Você pode enfrentar problemas de entrada ou de outro tipo, além de um domínio primário incorreto. Para resolver esse problema, talvez seja necessário mover os domínios para a rede correta com a ajuda do Suporte da Microsoft. Essa situação exige assistência direta e a solução pode demorar um pouco, especialmente se houver uma lista muito longa de nomes de domínio. Abra um caso de suporte para obter assistência na solução desses tipos de problemas.

Ao trabalhar com um agente de suporte, ele verificará se os domínios foram verificados em um locatário sob seu controle. Talvez ele faça outras perguntas de verificação sobre seus domínios, se eles foram adicionados ao locatário, mas não verificados pelo DNS. Certifique-se de que os domínios sejam verificados pelo DNS para acelerar o processo.
