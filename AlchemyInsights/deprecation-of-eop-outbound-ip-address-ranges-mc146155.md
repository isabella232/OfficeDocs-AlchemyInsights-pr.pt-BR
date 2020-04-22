---
title: 1065 substituição do endereço IP de saída EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704585"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Substituição dos intervalos de endereços IP de saída do EOP

Detectamos um possível problema com sua organização que (se não for corrigido por outubro de 26th, 2018) pode quebrar o fluxo de emails para seus destinos externos ou locais. Como comunicado anteriormente, para simplificar o gerenciamento do intervalo de endereços IP, estamos consolidando os intervalos de endereços IP do Exchange Online Protection (EOP) que são usados para enviar e receber emails fora do Microsoft 365. Nossa análise indica que uma ou mais fontes de email externas ou destinos que você configurou em conectores de fluxo de emails não estão aceitando conexões dos intervalos de endereços IP mostrados [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Atue antes de outubro de 26th para garantir que essas fontes e destinos aceitem conexões de e para todos os [endereços IP do EOP publicados](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Para obter mais informações sobre essa alteração, confira o centro de mensagens postagens [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Observação**: se você utilizou anteriormente a publicação de IP ou de URL via HTML, XML e RSS para atualizações de ponto de extremidade, também deverá migrar para os novos serviços Web para automatizar esses tipos de atualizações. Para obter mais informações, consulte [categorias de ponto de extremidade do microsoft 365 e endereço IP e URL do microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
