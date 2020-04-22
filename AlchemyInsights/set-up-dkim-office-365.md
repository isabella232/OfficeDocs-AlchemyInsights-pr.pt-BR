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
# <a name="setup-dkim"></a><span data-ttu-id="3f11d-102">Configurar DKIM</span><span class="sxs-lookup"><span data-stu-id="3f11d-102">Setup DKIM</span></span>

<span data-ttu-id="3f11d-103">As instruções completas para configurar o DKIM para domínios personalizados no Microsoft 365 estão [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="3f11d-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="3f11d-104">Para **cada** domínio personalizado, você precisa criar **dois** registros CNAME do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, o registrador de domínio).</span><span class="sxs-lookup"><span data-stu-id="3f11d-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="3f11d-105">Por exemplo, contoso.com e fourthcoffee.com exigem quatro registros CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="3f11d-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="3f11d-106">Os registros CNAME do DKIM para **cada** domínio personalizado usam os seguintes formatos:</span><span class="sxs-lookup"><span data-stu-id="3f11d-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="3f11d-107">**Nome do host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="3f11d-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="3f11d-108">**Aponta para o endereço ou o valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="3f11d-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="3f11d-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="3f11d-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="3f11d-110">**Nome do host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="3f11d-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="3f11d-111">**Aponta para o endereço ou o valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="3f11d-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="3f11d-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="3f11d-112">**TTL**: 3600</span></span>

   <span data-ttu-id="3f11d-113">\<DomainGUID\> é o texto à esquerda do `.mail.protection.outlook.com` registro MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3f11d-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="3f11d-114">\<InitialDomain\> é o domínio que você usou ao se inscrever no Microsoft 365 (por exemplo, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="3f11d-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="3f11d-115">Depois de criar os registros CNAME para seus domínios personalizados, conclua as instruções a seguir:</span><span class="sxs-lookup"><span data-stu-id="3f11d-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="3f11d-116">a.</span><span class="sxs-lookup"><span data-stu-id="3f11d-116">a.</span></span> <span data-ttu-id="3f11d-117">[entre no Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com sua conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="3f11d-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="3f11d-118">b.</span><span class="sxs-lookup"><span data-stu-id="3f11d-118">b.</span></span> <span data-ttu-id="3f11d-119">Selecione o ícone do inicializador de aplicativos no canto superior esquerdo e escolha **Administrador**.</span><span class="sxs-lookup"><span data-stu-id="3f11d-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="3f11d-120">c.</span><span class="sxs-lookup"><span data-stu-id="3f11d-120">c.</span></span> <span data-ttu-id="3f11d-121">No painel de navegação inferior à esquerda, expanda **Administrador** e escolha **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="3f11d-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="3f11d-122">d.</span><span class="sxs-lookup"><span data-stu-id="3f11d-122">d.</span></span> <span data-ttu-id="3f11d-123">Vá para **Protection** > **DKIM**de proteção.</span><span class="sxs-lookup"><span data-stu-id="3f11d-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="3f11d-124">e.</span><span class="sxs-lookup"><span data-stu-id="3f11d-124">e.</span></span> <span data-ttu-id="3f11d-125">Selecione o domínio e, em seguida, escolha **habilitar** para **assinar mensagens para este domínio com assinaturas do DKIM**.</span><span class="sxs-lookup"><span data-stu-id="3f11d-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="3f11d-126">Repita essa etapa para cada domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="3f11d-126">Repeat this step for each custom domain.</span></span>
