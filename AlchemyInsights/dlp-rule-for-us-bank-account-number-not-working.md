---
title: Regra de DLP para nós número de conta bancária não funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916404"
---
<span data-ttu-id="f277e-p101">Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo que contém um **Número de conta bancária EUA** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, verifique se seu conteúdo contém as informações necessárias para que a política de DLP está procurando por quando ele é avaliado.</span><span class="sxs-lookup"><span data-stu-id="f277e-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="f277e-104">Por exemplo, para uma política de **Número de conta bancária US** configurada com um nível de confiança de 85%, o seguinte é avaliado e deve ser detectado para acionar a regra:</span><span class="sxs-lookup"><span data-stu-id="f277e-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="f277e-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 17 de 8 dígitos</span><span class="sxs-lookup"><span data-stu-id="f277e-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="f277e-106">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** dígitos consecutivos de 8-17.</span><span class="sxs-lookup"><span data-stu-id="f277e-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="f277e-107">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há nenhuma soma de verificação</span><span class="sxs-lookup"><span data-stu-id="f277e-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="f277e-108">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política de DLP é 75% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="f277e-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="f277e-109">A expressão regular Regex_usa_bank_account_number encontra o conteúdo que corresponde ao padrão</span><span class="sxs-lookup"><span data-stu-id="f277e-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="f277e-110">Uma palavra-chave de Keyword_usa_Bank_Account for encontrada.</span><span class="sxs-lookup"><span data-stu-id="f277e-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="f277e-111">Por exemplo, o exemplo a seguir irá disparar para a política de **Número de conta bancária dos Estados Unidos** : conta corrente 78344011</span><span class="sxs-lookup"><span data-stu-id="f277e-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="f277e-112">Para obter mais informações sobre o que é necessário para um **Número de conta bancária nos EUA** a serem detectadas para o seu conteúdo, consulte a seção a seguir neste artigo: [O que o confidenciais tipos de informações procure o número de conta bancária dos EUA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="f277e-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="f277e-113">Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f277e-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

