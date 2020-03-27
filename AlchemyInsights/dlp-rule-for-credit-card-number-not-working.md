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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977186"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="a6f40-102">Problemas de DLP com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="a6f40-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="a6f40-103">**Importante**: durante esses horários sem precedentes, estamos executando etapas para garantir que o SharePoint Online e os serviços do onedrive permaneçam altamente disponíveis – visite [ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a6f40-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a6f40-104">**Problemas de DLP com números de cartão de crédito**</span><span class="sxs-lookup"><span data-stu-id="a6f40-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="a6f40-105">Você está tendo problemas com a **prevenção contra perda de dados (DLP)** não está funcionando para conteúdo que contém um **número de cartão de crédito** ao usar um tipo de informação confidencial de DLP no O365?</span><span class="sxs-lookup"><span data-stu-id="a6f40-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a6f40-106">Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para acionar a política de DLP quando for avaliada.</span><span class="sxs-lookup"><span data-stu-id="a6f40-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="a6f40-107">Por exemplo, para uma **política de cartão de crédito** configurada com um nível de confiança de 85%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada:</span><span class="sxs-lookup"><span data-stu-id="a6f40-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a6f40-108">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (dddddddddddddddd) e deve passar o teste Luhn.</span><span class="sxs-lookup"><span data-stu-id="a6f40-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="a6f40-109">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Um padrão muito complexo e robusto que detecta cartões de todas as principais marcas em todo o mundo, incluindo Visa, MasterCard, cartão de descoberta, JCB, American Express, Gift e cartões Diner.</span><span class="sxs-lookup"><span data-stu-id="a6f40-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="a6f40-110">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação Luhn</span><span class="sxs-lookup"><span data-stu-id="a6f40-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="a6f40-111">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP é de 85% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="a6f40-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a6f40-112">A função Func_credit_card localiza conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="a6f40-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a6f40-113">Uma das seguintes opções for verdadeira:</span><span class="sxs-lookup"><span data-stu-id="a6f40-113">One of the following is true:</span></span>

  - <span data-ttu-id="a6f40-114">Uma palavra-chave de Keyword_cc_verification for encontrada.</span><span class="sxs-lookup"><span data-stu-id="a6f40-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="a6f40-115">Uma palavra-chave de Keyword_cc_name for encontrada</span><span class="sxs-lookup"><span data-stu-id="a6f40-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="a6f40-116">A função Func_expiration_date encontra uma data no formato de data à direita.</span><span class="sxs-lookup"><span data-stu-id="a6f40-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="a6f40-117">O checksum passa</span><span class="sxs-lookup"><span data-stu-id="a6f40-117">The checksum passes</span></span>

    <span data-ttu-id="a6f40-118">Por exemplo, o exemplo a seguir é disparado para uma política de número de cartão de crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="a6f40-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="a6f40-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="a6f40-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="a6f40-120">Expira em: 2/2009</span><span class="sxs-lookup"><span data-stu-id="a6f40-120">Expires: 2/2009</span></span>

<span data-ttu-id="a6f40-121">Para obter mais informações sobre o que é necessário para que um **número de cartão de crédito** seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram por cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a6f40-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="a6f40-122">Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a6f40-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  