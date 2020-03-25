---
title: Dicas de política de DLP que não funcionam
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932574"
---
# <a name="dlp-policy-tip-issues"></a>Problemas de dica de política DLP

**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano. Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup. Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.

Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana. Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período. No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.

**Dicas de política de DLP**

Ao usar **políticas DLP**, os usuários podem ser notificados de uma violação de política com **dicas de política**. Os administradores podem configurar dicas de política para exibir durante o teste da política de DLP ou quando a política está no modo de imposição total.
  
Para configurar dicas de política em sua política de DLP no centro de segurança e conformidade no modo de imposição completa, faça o seguinte:
  
- Verifique se as dicas de política foram **habilitadas** na regra DLP usando as etapas [aqui](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Verifique se o **conteúdo corresponde** ao que é **necessário** para acionar a regra descrita neste artigo [aqui](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- As dicas de política são exibidas no OWA e no Outlook. No entanto, ao usar o **Outlook 2013 ou posterior**, as dicas de política são exibidas apenas em determinadas condições. Essas condições estão listadas aqui: [condições suportadas para o Outlook 2013 ou posterior para exibir dicas de política](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Para obter informações adicionais sobre dicas de política de DLP, consulte: [Mostrar dicas de política para políticas de DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  