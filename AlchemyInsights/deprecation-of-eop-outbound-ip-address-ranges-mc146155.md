---
title: 1065 substituição do endereço IP de saída EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777260"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7cfb7-102">Substituição dos intervalos de endereços IP de saída do EOP</span><span class="sxs-lookup"><span data-stu-id="7cfb7-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7cfb7-103">Detectamos um possível problema com sua organização que (se não for corrigido por outubro de 26th, 2018) pode quebrar o fluxo de emails para seus destinos externos ou locais.</span><span class="sxs-lookup"><span data-stu-id="7cfb7-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7cfb7-104">Como comunicado anteriormente, para simplificar o gerenciamento do intervalo de endereços IP, estamos consolidando os intervalos de endereços IP do Exchange Online Protection (EOP) que são usados para enviar e receber emails fora do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7cfb7-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="7cfb7-105">Nossa análise indica que uma ou mais fontes de email externas ou destinos que você configurou em conectores de fluxo de emails não estão aceitando conexões dos intervalos de endereços IP mostrados [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7cfb7-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7cfb7-106">Atue antes de outubro de 26th para garantir que essas fontes e destinos aceitem conexões de e para todos os [endereços IP do EOP publicados](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7cfb7-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7cfb7-107">Para obter mais informações sobre essa alteração, confira o centro de mensagens postagens [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7cfb7-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="7cfb7-108">**Observação**: se você utilizou anteriormente a publicação de IP ou de URL via HTML, XML e RSS para atualizações de ponto de extremidade, também deverá migrar para os novos serviços Web para automatizar esses tipos de atualizações.</span><span class="sxs-lookup"><span data-stu-id="7cfb7-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7cfb7-109">Para obter mais informações, consulte [categorias de ponto de extremidade do office 365 e endereço IP e URL 365 do Office](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7cfb7-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

