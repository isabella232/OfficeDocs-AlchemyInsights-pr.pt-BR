---
title: 1065 substituição do endereço IP de saída EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752943"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Substituição dos intervalos de endereços IP de saída do EOP

Detectamos um possível problema com sua organização que (se não for corrigido por outubro de 26th, 2018) pode quebrar o fluxo de emails para seus destinos externos ou locais. Como comunicado anteriormente, para simplificar o gerenciamento do intervalo de endereços IP, estamos consolidando os intervalos de endereços IP do Exchange Online Protection (EOP) que são usados para enviar e receber emails fora do Office 365. Nossa análise indica que uma ou mais fontes de email externas ou destinos que você configurou em conectores de fluxo de emails não estão aceitando conexões dos intervalos de endereços IP mostrados [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Atue antes de outubro de 26th para garantir que essas fontes e destinos aceitem conexões de e para todos os [endereços IP do EOP publicados](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Para obter mais informações sobre essa alteração, confira o centro de mensagens postagens [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Observação**: se você utilizou anteriormente a publicação de IP ou de URL via HTML, XML e RSS para atualizações de ponto de extremidade, também deverá migrar para os novos serviços Web para automatizar esses tipos de atualizações. Para obter mais informações, consulte [categorias de ponto de extremidade do office 365 e endereço IP e URL 365 do Office](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
