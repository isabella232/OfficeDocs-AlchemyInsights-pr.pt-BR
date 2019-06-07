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
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="2b5cd-102">Configurar o DKIM no Office 365</span><span class="sxs-lookup"><span data-stu-id="2b5cd-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="2b5cd-103">As instruções completas para configurar o DKIM para domínios personalizados no Office 365 estão [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2b5cd-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="2b5cd-104">Para **cada** domínio personalizado, você precisa criar **dois** registros CNAME do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, o registrador de domínio).</span><span class="sxs-lookup"><span data-stu-id="2b5cd-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="2b5cd-105">Por exemplo, contoso.com e fourthcoffee.com exigem quatro registros CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="2b5cd-106">Os registros CNAME do DKIM para **cada** domínio personalizado usam os seguintes formatos:</span><span class="sxs-lookup"><span data-stu-id="2b5cd-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="2b5cd-107">**Nome do host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2b5cd-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2b5cd-108">**Aponta para o endereço ou o valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2b5cd-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2b5cd-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2b5cd-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="2b5cd-110">**Nome do host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2b5cd-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2b5cd-111">**Aponta para o endereço ou o valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2b5cd-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2b5cd-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2b5cd-112">**TTL**: 3600</span></span>

   <span data-ttu-id="2b5cd-113">\<DomainGUID\> é o texto à esquerda do `.mail.protection.outlook.com` registro MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2b5cd-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="2b5cd-114">\<InitialDomain\> é o domínio que você usou ao se inscrever no Office 365 (por exemplo, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="2b5cd-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="2b5cd-115">Depois de criar os registros CNAME para seus domínios personalizados, conclua as instruções a seguir:</span><span class="sxs-lookup"><span data-stu-id="2b5cd-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="2b5cd-116">a.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-116">a.</span></span> <span data-ttu-id="2b5cd-117">[Entre no Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com sua conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="2b5cd-118">b.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-118">b.</span></span> <span data-ttu-id="2b5cd-119">Selecione o ícone do inicializador de aplicativos no canto superior esquerdo e escolha **Administrador**.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="2b5cd-120">c.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-120">c.</span></span> <span data-ttu-id="2b5cd-121">No painel de navegação inferior à esquerda, expanda **Administrador** e escolha **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="2b5cd-122">d.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-122">d.</span></span> <span data-ttu-id="2b5cd-123">Vá para \*\*\*\* > **DKIM**de proteção.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="2b5cd-124">e.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-124">e.</span></span> <span data-ttu-id="2b5cd-125">Selecione o domínio e, em seguida, escolha **habilitar** para **assinar mensagens para este domínio com assinaturas do DKIM**.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="2b5cd-126">Repita essa etapa para cada domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="2b5cd-126">Repeat this step for each custom domain.</span></span>
