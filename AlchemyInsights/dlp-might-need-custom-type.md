---
title: A DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932646"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="f2b26-102">A DLP pode precisar de um tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="f2b26-102">DLP might need a custom type</span></span>

<span data-ttu-id="f2b26-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="f2b26-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f2b26-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="f2b26-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f2b26-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="f2b26-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f2b26-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="f2b26-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f2b26-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="f2b26-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f2b26-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="f2b26-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f2b26-109">**A DLP pode exigir um tipo de informação personalizado**</span><span class="sxs-lookup"><span data-stu-id="f2b26-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="f2b26-110">Com uma política de prevenção de perda de dados (DLP), você pode identificar e proteger dados confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="f2b26-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="f2b26-111">Em alguns cenários, talvez seja necessário criar seu próprio tipo **personalizado** de informações confidenciais para proteger os dados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="f2b26-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="f2b26-112">Por exemplo, sua organização pode precisar identificar e proteger IDs de funcionários ou outros dados em um formato específico para sua organização. Em caso afirmativo, consulte os artigos a seguir para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f2b26-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="f2b26-113">**Personalizar um tipo de informação confidencial interno**</span><span class="sxs-lookup"><span data-stu-id="f2b26-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="f2b26-114">Se um tipo de informação confidencial interno atender às suas necessidades com apenas alguns ajustes, você poderá [Personalizar um tipo de informação confidencial interno](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f2b26-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="f2b26-115">Por exemplo, você pode adicionar ou remover palavras-chave ou adicionar ou remover evidências de suporte, como uma data ou um endereço.</span><span class="sxs-lookup"><span data-stu-id="f2b26-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="f2b26-116">**Criar um tipo de informação confidencial personalizado**</span><span class="sxs-lookup"><span data-stu-id="f2b26-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="f2b26-117">Mas se você precisar identificar e proteger um tipo diferente de informações confidenciais, poderá [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na interface do usuário do centro de conformidade de & de segurança.</span><span class="sxs-lookup"><span data-stu-id="f2b26-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="f2b26-118">**Crie um tipo personalizado de informação confidencial no PowerShell do Centro de Conformidade e Segurança**</span><span class="sxs-lookup"><span data-stu-id="f2b26-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="f2b26-119">Por fim, se a interface do usuário não fornecer todas as opções necessárias, você poderá [criar um tipo de informação confidencial personalizado no PowerShell do centro de conformidade e segurança &](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="f2b26-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="f2b26-120">A partir de um arquivo XML, você pode usar todas as opções disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f2b26-120">By starting with an XML file, you can use every option available.</span></span>
