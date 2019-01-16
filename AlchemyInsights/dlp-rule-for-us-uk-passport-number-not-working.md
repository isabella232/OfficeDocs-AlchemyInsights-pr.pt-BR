---
title: Regra DLP para EUA / número de passaporte do Reino Unido não funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275362"
---
<span data-ttu-id="8f1ab-p101">Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo contendo um **US / número de passaporte do Reino Unido** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, verifique se seu conteúdo contém as informações necessárias para que a política de DLP está procurando por quando ele é avaliado.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="8f1ab-104">Por exemplo, para um **US / número de passaporte do Reino Unido** política configurada com um nível de confiança de 75%, o seguinte é avaliado e devem ser detectado para acionar a regra</span><span class="sxs-lookup"><span data-stu-id="8f1ab-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="8f1ab-105">**[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos</span><span class="sxs-lookup"><span data-stu-id="8f1ab-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="8f1ab-106">**[Padrão:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos</span><span class="sxs-lookup"><span data-stu-id="8f1ab-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="8f1ab-107">**[Soma de verificação:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há nenhuma soma de verificação</span><span class="sxs-lookup"><span data-stu-id="8f1ab-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="8f1ab-108">**[Definição:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP é 75% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="8f1ab-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="8f1ab-109">A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="8f1ab-110">Uma palavra-chave de Keyword_passport for encontrada.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="8f1ab-111">Por exemplo, o exemplo a seguir irá disparar para o **US / número de passaporte do Reino Unido** política: número de passaporte US 123456789</span><span class="sxs-lookup"><span data-stu-id="8f1ab-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="8f1ab-112">Para obter mais informações sobre o que é necessário para um EUA / número de passaporte do Reino Unido a serem detectadas para seu conteúdo, consulte a seção a seguir neste artigo: [aparência do qual o confidenciais tipos de informações para US / número de passaporte do Reino Unido](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="8f1ab-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="8f1ab-113">Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="8f1ab-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

