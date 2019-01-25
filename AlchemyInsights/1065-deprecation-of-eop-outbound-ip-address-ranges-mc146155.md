---
title: RangesMC146155 1065 endereço IP, saída preterir do EOP
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457376"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Preterir de intervalos de endereços IP saídos EOP

Podemos foi detectado um possível problema com a sua organização que (se não corrigido por 26 de outubro de 2018) pode interromper o fluxo de email ao seu local ou destinos externos. Como anteriormente comunicados, para simplificar o gerenciamento de intervalo de endereços IP, estamos consolidando os intervalos de endereços IP do Exchange Online Protection (EOP) que são usados para enviar e receber emails fora do Office 365. Nossa análise indica que uma ou mais fontes de email externo ou destinos que você configurou nos conectores de fluxo de email não aceitação mais conexões do IP endereço intervalos mostrado [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Atuar antes de 26 de outubro para garantir que essas fontes e destinos aceitará conexões de e para todos os [endereços IP do EOP de publicado](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Para obter mais informações sobre essa alteração, consulte a que Central de mensagens postagens [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Observação**: se você já utilizou o IP ou URL publicação via RSS, XML e HTML para atualizações do ponto de extremidade, você também deve migrar para os novos serviços da web para automatizar esses tipos de atualizações. Para obter mais informações, consulte [categorias de ponto de extremidade do Office 365 e o endereço de IP do Office 365 e o URL do serviço web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

