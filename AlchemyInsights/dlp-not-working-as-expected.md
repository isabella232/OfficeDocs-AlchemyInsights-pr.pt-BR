---
title: DLP não está funcionando conforme esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977426"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="d33ed-102">DLP não está funcionando conforme esperado</span><span class="sxs-lookup"><span data-stu-id="d33ed-102">DLP not working as expected</span></span>

<span data-ttu-id="d33ed-103">**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="d33ed-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="d33ed-104">**Configurando DLP**</span><span class="sxs-lookup"><span data-stu-id="d33ed-104">**Setting up DLP**</span></span>

<span data-ttu-id="d33ed-105">Você está tendo problemas com a **prevenção de perda de dados (DLP)** no Office 365 que não está funcionando conforme o esperado?</span><span class="sxs-lookup"><span data-stu-id="d33ed-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="d33ed-106">Em caso afirmativo, certifique-se de que sua **política de DLP** está configurada corretamente e que seus dados contêm o que a **política de DLP** está procurando quando estiver sendo avaliada.</span><span class="sxs-lookup"><span data-stu-id="d33ed-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="d33ed-107">As políticas de DLP permitem identificar e proteger informações confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d33ed-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="d33ed-108">Para configurar as políticas de DLP, use as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="d33ed-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="d33ed-109">**O que as políticas de DLP procuram**</span><span class="sxs-lookup"><span data-stu-id="d33ed-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="d33ed-110">Ao usar os **tipos de informações confidenciais internas** no centro de segurança e conformidade do Office 365, as políticas de DLP procuram padrões e elementos específicos ao detectar esses tipos confidenciais.</span><span class="sxs-lookup"><span data-stu-id="d33ed-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="d33ed-111">**Tipos de informações confidenciais internas**</span><span class="sxs-lookup"><span data-stu-id="d33ed-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="d33ed-112">Para obter informações sobre os tipos confidenciais internos e o que a política de DLP procura ao detectar o tipo confidencial, consulte: [o que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="d33ed-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="d33ed-113">**Tipos de informações confidenciais personalizadas**</span><span class="sxs-lookup"><span data-stu-id="d33ed-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="d33ed-114">Se você estiver tentando criar tipos de informações confidenciais personalizados, use o artigo a seguir para obter informações sobre como criar um tipo confidencial personalizado: [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d33ed-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="d33ed-115">**Testar uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="d33ed-115">**Test a DLP policy**</span></span>

<span data-ttu-id="d33ed-116">Para testar seus dados com um tipo de informação confidencial interno ou personalizado, use a opção **tipo de teste** em **classificações** > **confidenciais tipos de informações**.</span><span class="sxs-lookup"><span data-stu-id="d33ed-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="d33ed-117">Para obter mais informações, consulte [testar tipos de informações confidenciais personalizados](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="d33ed-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="d33ed-118">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="d33ed-118">**Reports**</span></span>
  
- <span data-ttu-id="d33ed-119">Obtenha informações confidenciais sobre os relatórios de [DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="d33ed-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="d33ed-120">Veja detalhes específicos do evento com um [relatório de incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="d33ed-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
