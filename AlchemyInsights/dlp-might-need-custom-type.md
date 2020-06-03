---
title: A DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507502"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="35466-102">A DLP pode precisar de um tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="35466-102">DLP might need a custom type</span></span>

<span data-ttu-id="35466-103">**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="35466-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="35466-104">**A DLP pode exigir um tipo de informação personalizado**</span><span class="sxs-lookup"><span data-stu-id="35466-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="35466-105">Com uma política de prevenção de perda de dados (DLP), você pode identificar e proteger dados confidenciais em sua organização.</span><span class="sxs-lookup"><span data-stu-id="35466-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="35466-106">Em alguns cenários, talvez seja necessário criar seu próprio tipo **personalizado** de informações confidenciais para proteger os dados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="35466-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="35466-107">Por exemplo, sua organização pode precisar identificar e proteger IDs de funcionários ou outros dados em um formato específico para sua organização. Em caso afirmativo, consulte os artigos a seguir para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="35466-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="35466-108">**Personalizar um tipo de informação confidencial interno**</span><span class="sxs-lookup"><span data-stu-id="35466-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="35466-109">Se um tipo de informação confidencial interno atender às suas necessidades com apenas alguns ajustes, você poderá [Personalizar um tipo de informação confidencial interno](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="35466-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="35466-110">Por exemplo, você pode adicionar ou remover palavras-chave ou adicionar ou remover evidências de suporte, como uma data ou um endereço.</span><span class="sxs-lookup"><span data-stu-id="35466-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="35466-111">**Criar um tipo de informação confidencial personalizado**</span><span class="sxs-lookup"><span data-stu-id="35466-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="35466-112">Mas se você precisar identificar e proteger um tipo diferente de informações confidenciais, poderá [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) na interface do usuário do centro de conformidade de & de segurança.</span><span class="sxs-lookup"><span data-stu-id="35466-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="35466-113">**Crie um tipo personalizado de informação confidencial no PowerShell do Centro de Conformidade e Segurança**</span><span class="sxs-lookup"><span data-stu-id="35466-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="35466-114">Por fim, se a interface do usuário não fornecer todas as opções necessárias, você poderá [criar um tipo de informação confidencial personalizado no PowerShell do centro de conformidade e segurança &](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="35466-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="35466-115">A partir de um arquivo XML, você pode usar todas as opções disponíveis.</span><span class="sxs-lookup"><span data-stu-id="35466-115">By starting with an XML file, you can use every option available.</span></span>
