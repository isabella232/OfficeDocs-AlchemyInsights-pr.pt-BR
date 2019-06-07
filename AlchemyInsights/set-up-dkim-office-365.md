---
title: Configurar o DKIM no Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764835"
---
# <a name="setup-dkim-in-office-365"></a>Configurar o DKIM no Office 365

As instruções completas para configurar o DKIM para domínios personalizados no Office 365 estão [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Para **cada** domínio personalizado, você precisa criar **dois** registros CNAME do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, o registrador de domínio). Por exemplo, contoso.com e fourthcoffee.com exigem quatro registros CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.

   Os registros CNAME do DKIM para **cada** domínio personalizado usam os seguintes formatos:

   - **Nome do host**:`selector1._domainkey.<CustomDomain>`

     **Aponta para o endereço ou o valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome do host**:`selector2._domainkey.<CustomDomain>`

     **Aponta para o endereço ou o valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> é o texto à esquerda do `.mail.protection.outlook.com` registro MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com). \<InitialDomain\> é o domínio que você usou ao se inscrever no Office 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de criar os registros CNAME para seus domínios personalizados, conclua as instruções a seguir:

   a. [Entre no Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com sua conta corporativa ou de estudante.

   b. Selecione o ícone do inicializador de aplicativos no canto superior esquerdo e escolha **Administrador**.

   c. No painel de navegação inferior à esquerda, expanda **Administrador** e escolha **Exchange**.

   d. Vá para **** > **DKIM**de proteção.

   e. Selecione o domínio e, em seguida, escolha **habilitar** para **assinar mensagens para este domínio com assinaturas do DKIM**. Repita essa etapa para cada domínio personalizado.
