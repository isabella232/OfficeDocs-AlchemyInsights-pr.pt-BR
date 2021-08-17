---
title: Configurar O DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108544"
---
# <a name="setup-dkim"></a>Configurar O DKIM

As instruções completas para configurar o DKIM para domínios personalizados Microsoft 365 estão [aqui](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Para **cada** domínio personalizado, você precisa criar dois registros **CNAME** DKIM no serviço de hospedagem DNS do seu domínio (normalmente, o registrador de domínios). Por exemplo, contoso.com e fourthcoffee.com exigem quatro registros CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.

   Os registros CNAME DKIM para **cada** domínio personalizado usam os seguintes formatos:

   - **Nome do host**: `selector1._domainkey.<CustomDomain>`

     **Pontos para endereço ou valor:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome do host**: `selector2._domainkey.<CustomDomain>`

     **Pontos para endereço ou valor:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> é o texto à esquerda do registro MX personalizado para o domínio personalizado (por exemplo, para o domínio `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>é o domínio usado quando você se inscreveu para Microsoft 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de criar os registros CNAME para seus domínios personalizados, conclua as seguintes instruções:

   a. [entre no Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com sua conta de trabalho ou de estudante.

   b. Selecione o ícone do inicializador de aplicativos no canto superior esquerdo e escolha **Administrador**.

   c. No painel de navegação inferior à esquerda, expanda **Administrador** e escolha **Exchange**.

   d. Vá para **Proteção**  >  **DKIM**.

   e. Selecione o domínio e escolha **Habilitar** para **Assinar mensagens para este domínio com assinaturas DKIM**. Repita essa etapa para cada domínio personalizado.
