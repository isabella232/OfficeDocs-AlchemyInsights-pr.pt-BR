---
title: Regra de DLP para número de cartão de crédito não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932431"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="9e839-102">Problemas de DLP com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="9e839-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="9e839-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="9e839-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9e839-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="9e839-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9e839-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="9e839-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9e839-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="9e839-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9e839-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="9e839-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9e839-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="9e839-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9e839-109">**Problemas de DLP com números de cartão de crédito**</span><span class="sxs-lookup"><span data-stu-id="9e839-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="9e839-110">Você está tendo problemas com a **prevenção contra perda de dados (DLP)** não está funcionando para conteúdo que contém um **número de cartão de crédito** ao usar um tipo de informação confidencial de DLP no O365?</span><span class="sxs-lookup"><span data-stu-id="9e839-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9e839-111">Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para acionar a política de DLP quando for avaliada.</span><span class="sxs-lookup"><span data-stu-id="9e839-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="9e839-112">Por exemplo, para uma **política de cartão de crédito** configurada com um nível de confiança de 85%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada:</span><span class="sxs-lookup"><span data-stu-id="9e839-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9e839-113">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (dddddddddddddddd) e deve passar o teste Luhn.</span><span class="sxs-lookup"><span data-stu-id="9e839-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="9e839-114">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Um padrão muito complexo e robusto que detecta cartões de todas as principais marcas em todo o mundo, incluindo Visa, MasterCard, cartão de descoberta, JCB, American Express, Gift e cartões Diner.</span><span class="sxs-lookup"><span data-stu-id="9e839-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="9e839-115">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação Luhn</span><span class="sxs-lookup"><span data-stu-id="9e839-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="9e839-116">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP é de 85% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="9e839-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9e839-117">A função Func_credit_card localiza conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="9e839-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9e839-118">Uma das seguintes opções for verdadeira:</span><span class="sxs-lookup"><span data-stu-id="9e839-118">One of the following is true:</span></span>

  - <span data-ttu-id="9e839-119">Uma palavra-chave de Keyword_cc_verification for encontrada.</span><span class="sxs-lookup"><span data-stu-id="9e839-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="9e839-120">Uma palavra-chave de Keyword_cc_name for encontrada</span><span class="sxs-lookup"><span data-stu-id="9e839-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="9e839-121">A função Func_expiration_date encontra uma data no formato de data à direita.</span><span class="sxs-lookup"><span data-stu-id="9e839-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="9e839-122">O checksum passa</span><span class="sxs-lookup"><span data-stu-id="9e839-122">The checksum passes</span></span>

    <span data-ttu-id="9e839-123">Por exemplo, o exemplo a seguir é disparado para uma política de número de cartão de crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="9e839-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="9e839-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="9e839-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="9e839-125">Expira em: 2/2009</span><span class="sxs-lookup"><span data-stu-id="9e839-125">Expires: 2/2009</span></span>

<span data-ttu-id="9e839-126">Para obter mais informações sobre o que é necessário para que um **número de cartão de crédito** seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram por cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="9e839-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="9e839-127">Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="9e839-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  