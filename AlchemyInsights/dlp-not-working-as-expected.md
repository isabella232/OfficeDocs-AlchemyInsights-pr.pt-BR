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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530267"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="7e453-102">DLP não está funcionando conforme esperado</span><span class="sxs-lookup"><span data-stu-id="7e453-102">DLP not working as expected</span></span>

<span data-ttu-id="7e453-103">Você está tendo problemas com a **prevenção de perda de dados (DLP)** no Office 365 que não está funcionando conforme o esperado?</span><span class="sxs-lookup"><span data-stu-id="7e453-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="7e453-104">Em caso afirmativo, certifique-se de que sua **política de DLP** está configurada corretamente e que seus dados contêm o que a **política de DLP** está procurando quando estiver sendo avaliada.</span><span class="sxs-lookup"><span data-stu-id="7e453-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="7e453-105">**Configurando DLP**</span><span class="sxs-lookup"><span data-stu-id="7e453-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="7e453-106">As políticas de DLP permitem identificar e proteger informações confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="7e453-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="7e453-107">Para configurar as políticas de DLP, use as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="7e453-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="7e453-108">**O que as políticas de DLP procuram**</span><span class="sxs-lookup"><span data-stu-id="7e453-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="7e453-109">Ao usar os **tipos de informações confidenciais internas** no centro de segurança e conformidade do Office 365, as políticas de DLP procuram padrões e elementos específicos ao detectar esses tipos confidenciais.</span><span class="sxs-lookup"><span data-stu-id="7e453-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="7e453-110">**Tipos de informações confidenciais internas**</span><span class="sxs-lookup"><span data-stu-id="7e453-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="7e453-111">Para obter informações sobre os tipos confidenciais internos e o que a política de DLP procura ao detectar o tipo confidencial, consulte: [o que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="7e453-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="7e453-112">**Tipos de informações confidenciais personalizadas**</span><span class="sxs-lookup"><span data-stu-id="7e453-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="7e453-113">Se você estiver tentando criar tipos de informações confidenciais personalizados, use o artigo a seguir para obter informações sobre como criar um tipo confidencial personalizado: [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="7e453-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="7e453-114">**Testar uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="7e453-114">**Test a DLP policy**</span></span>

<span data-ttu-id="7e453-115">Para testar seus dados com um tipo de informação confidencial interno ou personalizado, use a opção **tipo de teste** em **classificações** > **confidenciais tipos de informações**.</span><span class="sxs-lookup"><span data-stu-id="7e453-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7e453-116">Para obter mais informações, consulte [testar tipos de informações confidenciais personalizados](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7e453-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="7e453-117">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="7e453-117">**Reports**</span></span>
  
- <span data-ttu-id="7e453-118">Obtenha informações confidenciais sobre os relatórios de [DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="7e453-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="7e453-119">Veja detalhes específicos do evento com um [relatório de incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="7e453-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
