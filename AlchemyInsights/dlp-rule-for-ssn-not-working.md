---
title: A regra de DLP para SSN não está funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788690"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="1dadd-102">Problemas de DLP com números de segurança social</span><span class="sxs-lookup"><span data-stu-id="1dadd-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="1dadd-103">**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="1dadd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1dadd-104">**Problemas de DLP com o CPFs**</span><span class="sxs-lookup"><span data-stu-id="1dadd-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="1dadd-105">Você está tendo problemas com a **prevenção de perda de dados (DLP)** que não está funcionando para conteúdo que contém um **número de seguridade social (SSN)** ao usar um tipo de informação confidencial no Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="1dadd-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="1dadd-106">Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para o que a política de DLP está procurando.</span><span class="sxs-lookup"><span data-stu-id="1dadd-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="1dadd-107">Por exemplo, para uma política de SSN configurada com um nível de confiança de 85%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada:</span><span class="sxs-lookup"><span data-stu-id="1dadd-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1dadd-108">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 dígitos, que podem estar em um padrão formatado ou não formatado</span><span class="sxs-lookup"><span data-stu-id="1dadd-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="1dadd-109">**[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram CPFs em quatro padrões diferentes:</span><span class="sxs-lookup"><span data-stu-id="1dadd-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="1dadd-110">Func_ssn localiza CPFs com formatação forte de 2011 formatada com traços ou espaços (DDD-DD-dddd ou DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="1dadd-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="1dadd-111">Func_unformatted_ssn localiza CPFs com uma formatação forte anterior à 2011 que não são formatadas como nove dígitos consecutivos (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="1dadd-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="1dadd-112">Func_randomized_formatted_ssn localiza CPFs post-2011 que são formatados com traços ou espaços (DDD-DD-dddd ou DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="1dadd-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="1dadd-113">Func_randomized_unformatted_ssn localiza CPFs post-2011 que não estão formatados como nove dígitos consecutivos (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="1dadd-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="1dadd-114">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Não, não há checksum</span><span class="sxs-lookup"><span data-stu-id="1dadd-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="1dadd-115">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Uma política de DLP é de 85% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="1dadd-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1dadd-116">A [função Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) localiza o conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="1dadd-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="1dadd-117">Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) for encontrada.</span><span class="sxs-lookup"><span data-stu-id="1dadd-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="1dadd-118">Exemplos de palavras-chave incluem: *Social Security, Social Security #, SOC SEC, ssn* .</span><span class="sxs-lookup"><span data-stu-id="1dadd-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="1dadd-119">Por exemplo, o exemplo a seguir é disparado para a política de SSN do SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="1dadd-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="1dadd-120">Para obter mais informações sobre o que é necessário para que o CPFs seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram CPFs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="1dadd-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="1dadd-121">Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1dadd-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  