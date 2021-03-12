---
title: A DLP não está funcionando conforme o esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707798"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="7d0e4-102">A DLP não está funcionando conforme o esperado</span><span class="sxs-lookup"><span data-stu-id="7d0e4-102">DLP not working as expected</span></span>

<span data-ttu-id="7d0e4-103">**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7d0e4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="7d0e4-104">**Configuração de DLP**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-104">**Setting up DLP**</span></span>

<span data-ttu-id="7d0e4-105">Você está com problemas com a Prevenção contra Perda de Dados **(DLP)** no Office 365 não está funcionando conforme o esperado?</span><span class="sxs-lookup"><span data-stu-id="7d0e4-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="7d0e4-106">Nesse caso, certifique-se de que sua política **de DLP** está configurada corretamente e que seus dados contenham o que a **política de DLP** está procurando quando ela está sendo avaliada.</span><span class="sxs-lookup"><span data-stu-id="7d0e4-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="7d0e4-107">As políticas DLP permitem identificar e proteger informações confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="7d0e4-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="7d0e4-108">Para configurar políticas de DLP, use as informações [aqui](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="7d0e4-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="7d0e4-109">**O que as políticas de DLP procurar**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="7d0e4-110">Ao usar os **tipos de** informações confidenciais internas nos centros de Segurança e Conformidade, as políticas DLP procurarão padrões e elementos específicos ao detectar esses tipos confidenciais.</span><span class="sxs-lookup"><span data-stu-id="7d0e4-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="7d0e4-111">**Tipos de informações confidenciais integrados**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="7d0e4-112">Para obter informações sobre os tipos Confidenciais integrados e o que uma política DLP procura ao detectar o tipo Sensitive, consulte: O que os tipos de informações confidenciais [procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="7d0e4-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="7d0e4-113">**Tipos de informações confidenciais personalizados**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="7d0e4-114">Se você estiver tentando criar tipos de informações confidenciais personalizados, use o seguinte artigo para obter informações sobre como criar um tipo personalizado de informação confidenciais: Criar um tipo de informação [personalizado e confidenciais.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="7d0e4-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="7d0e4-115">**Testar uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-115">**Test a DLP policy**</span></span>

<span data-ttu-id="7d0e4-116">Para testar seus dados com um tipo de informação confidenciais integrado ou personalizado, use a opção **Tipo** de teste em **Classificações** Tipos de informações  >  **confidenciais.**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7d0e4-117">Para obter mais informações, consulte [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7d0e4-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="7d0e4-118">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="7d0e4-118">**Reports**</span></span>
  
- <span data-ttu-id="7d0e4-119">Obter informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="7d0e4-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="7d0e4-120">Consulte detalhes específicos do evento com um [Relatório de Incidentes.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="7d0e4-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
