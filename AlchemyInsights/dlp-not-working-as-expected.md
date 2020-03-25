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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932610"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="1d9fc-102">DLP não está funcionando conforme esperado</span><span class="sxs-lookup"><span data-stu-id="1d9fc-102">DLP not working as expected</span></span>

<span data-ttu-id="1d9fc-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1d9fc-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1d9fc-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1d9fc-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1d9fc-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1d9fc-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="1d9fc-109">**Configurando DLP**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-109">**Setting up DLP**</span></span>

<span data-ttu-id="1d9fc-110">Você está tendo problemas com a **prevenção de perda de dados (DLP)** no Office 365 que não está funcionando conforme o esperado?</span><span class="sxs-lookup"><span data-stu-id="1d9fc-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="1d9fc-111">Em caso afirmativo, certifique-se de que sua **política de DLP** está configurada corretamente e que seus dados contêm o que a **política de DLP** está procurando quando estiver sendo avaliada.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="1d9fc-112">As políticas de DLP permitem identificar e proteger informações confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="1d9fc-113">Para configurar as políticas de DLP, use as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="1d9fc-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="1d9fc-114">**O que as políticas de DLP procuram**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="1d9fc-115">Ao usar os **tipos de informações confidenciais internas** no centro de segurança e conformidade do Office 365, as políticas de DLP procuram padrões e elementos específicos ao detectar esses tipos confidenciais.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="1d9fc-116">**Tipos de informações confidenciais internas**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="1d9fc-117">Para obter informações sobre os tipos confidenciais internos e o que a política de DLP procura ao detectar o tipo confidencial, consulte: [o que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="1d9fc-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="1d9fc-118">**Tipos de informações confidenciais personalizadas**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="1d9fc-119">Se você estiver tentando criar tipos de informações confidenciais personalizados, use o artigo a seguir para obter informações sobre como criar um tipo confidencial personalizado: [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1d9fc-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="1d9fc-120">**Testar uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-120">**Test a DLP policy**</span></span>

<span data-ttu-id="1d9fc-121">Para testar seus dados com um tipo de informação confidencial interno ou personalizado, use a opção **tipo de teste** em **classificações** > **confidenciais tipos de informações**.</span><span class="sxs-lookup"><span data-stu-id="1d9fc-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="1d9fc-122">Para obter mais informações, consulte [testar tipos de informações confidenciais personalizados](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="1d9fc-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="1d9fc-123">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="1d9fc-123">**Reports**</span></span>
  
- <span data-ttu-id="1d9fc-124">Obtenha informações confidenciais sobre os relatórios de [DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="1d9fc-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="1d9fc-125">Veja detalhes específicos do evento com um [relatório de incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="1d9fc-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
