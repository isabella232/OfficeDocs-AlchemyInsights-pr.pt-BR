---
title: Configurar DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645660"
---
# <a name="setup-dkim"></a>Configurar DKIM

As instruções completas para configurar o DKIM para domínios personalizados no Microsoft 365 estão [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Para **cada** domínio personalizado, você precisa criar **dois** registros CNAME do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, o registrador de domínio). Por exemplo, contoso.com e fourthcoffee.com exigem quatro registros CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.

   Os registros CNAME do DKIM para **cada** domínio personalizado usam os seguintes formatos:

   - **Nome do host**:`selector1._domainkey.<CustomDomain>`

     **Aponta para o endereço ou o valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome do host**:`selector2._domainkey.<CustomDomain>`

     **Aponta para o endereço ou o valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> é o texto à esquerda do `.mail.protection.outlook.com` registro MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com). \<InitialDomain\> é o domínio que você usou ao se inscrever no Microsoft 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de criar os registros CNAME para seus domínios personalizados, conclua as instruções a seguir:

   a. [entre no Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com sua conta corporativa ou de estudante.

   b. Selecione o ícone do inicializador de aplicativos no canto superior esquerdo e escolha **Administrador**.

   c. No painel de navegação inferior à esquerda, expanda **Administrador** e escolha **Exchange**.

   d. Vá para **Protection** > **DKIM**de proteção.

   e. Selecione o domínio e, em seguida, escolha **habilitar** para **assinar mensagens para este domínio com assinaturas do DKIM**. Repita essa etapa para cada domínio personalizado.
