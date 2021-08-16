---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031250"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Detectamos um possível problema com sua organização que (se não for corrigido até 26 de outubro de 2018) pode quebrar o fluxo de emails para seus destinos locais ou externos. Conforme comunicado anteriormente, para simplificar o gerenciamento do intervalo de endereços IP, estamos consolidando os intervalos de endereços IP Proteção do Exchange Online (EOP) usados para enviar e receber emails fora do Microsoft 365. Nossa análise indica que uma ou mais das fontes de email ou destinos externos que você configurou nos conectores de fluxo de emails não estão aceitando conexões dos intervalos de endereços IP mostrados [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Aja antes de 26 de outubro para garantir que essas fontes e destinos aceitem conexões de e de todos os endereços [IP EOP publicados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Para obter mais informações sobre essa alteração, consulte Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Observação**: se você usou publicações de IP ou URL anteriormente via HTML, XML e RSS para atualizações de ponto de extremidade, você também deve migrar para os novos serviços Web para automatizar esses tipos de atualizações. Para obter mais informações, [consulte Microsoft 365 endpoint categories e Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
