---
title: Regra de DLP para o número de cartão de crédito não funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919068"
---
<span data-ttu-id="8672b-p101">Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo que contém um **Número de cartão de crédito** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, certifique-se de seu conteúdo contém as informações necessárias para acionar a política de DLP quando ele é avaliado. Por exemplo, para uma **política de cartão de crédito** configurado com um nível de confiança de 85%, a seguir é avaliadas e deve ser detectadas para acionar a regra:</span><span class="sxs-lookup"><span data-stu-id="8672b-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="8672b-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatado (dddddddddddddddd) e deve passar o teste de Luhn.</span><span class="sxs-lookup"><span data-stu-id="8672b-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="8672b-106">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Muito complexa e robusto padrão que detecta cartões de todas as principais marcas nível mundiais, incluindo Visa, Mastercard, Discover Card, JCB, American Express, cartões de vale-presente e cartões de cliente.</span><span class="sxs-lookup"><span data-stu-id="8672b-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="8672b-107">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação Luhn</span><span class="sxs-lookup"><span data-stu-id="8672b-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="8672b-108">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política DLP é de 85% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="8672b-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="8672b-109">A função Func_credit_card localiza conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="8672b-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="8672b-110">Uma das seguintes opções for verdadeira:</span><span class="sxs-lookup"><span data-stu-id="8672b-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="8672b-111">Uma palavra-chave de Keyword_cc_verification for encontrada.</span><span class="sxs-lookup"><span data-stu-id="8672b-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="8672b-112">Uma palavra-chave da Keyword_cc_name for encontrada</span><span class="sxs-lookup"><span data-stu-id="8672b-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="8672b-113">A função Func_expiration_date encontra uma data no formato de data à direita.</span><span class="sxs-lookup"><span data-stu-id="8672b-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="8672b-114">Passa a soma de verificação</span><span class="sxs-lookup"><span data-stu-id="8672b-114">The checksum passes</span></span>
    
    <span data-ttu-id="8672b-115">Por exemplo, o exemplo a seguir irá disparar para uma política de número de cartão de crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="8672b-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="8672b-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="8672b-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="8672b-117">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="8672b-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="8672b-118">Para obter mais informações sobre o que é necessário para um **Número de cartão de crédito** a serem detectadas para o seu conteúdo, consulte a seção a seguir neste artigo: [O que o confidenciais tipos de informações procure o cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="8672b-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="8672b-119">Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="8672b-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

