---
title: Configurar o DKIM com domínios personalizados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500619"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurar o DKIM com domínios personalizados

Você deve publicar dois registros CNAME para cada domínio personalizado no DNS. Para fazer isso, use o seguinte formato:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** é o texto à esquerda de **.mail.protection.outlook.com** no registro MX personalizado para o domínio personalizado (por exemplo, contoso-com para o domínio **contoso.com**). **InitialDomain** é o domínio usado quando você se inscreveu no Office 365 (por exemplo, **contoso.onmicrosoft.com**).

Para obter mais informações sobre registros DNS, consulte [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).