---
title: Regra de DLP para o número do Passport US/Reino Unido que não está funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389529"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="dd114-102">Problemas com os números de passaporte do DLP-US/Reino Unido</span><span class="sxs-lookup"><span data-stu-id="dd114-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="dd114-103">Você está tendo problemas com a **prevenção de perda de dados (DLP)** que não está funcionando para conteúdo que contém um **número de passaporte US/Reino Unido** ao usar um tipo de informação confidencial de DLP no O365?</span><span class="sxs-lookup"><span data-stu-id="dd114-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dd114-104">Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para o que a política de DLP está procurando quando é avaliada.</span><span class="sxs-lookup"><span data-stu-id="dd114-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="dd114-105">Por exemplo, para uma política de **número de passaporte US/Reino Unido** configurada com um nível de confiança de 75%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada</span><span class="sxs-lookup"><span data-stu-id="dd114-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="dd114-106">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos</span><span class="sxs-lookup"><span data-stu-id="dd114-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="dd114-107">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos</span><span class="sxs-lookup"><span data-stu-id="dd114-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="dd114-108">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há checksum</span><span class="sxs-lookup"><span data-stu-id="dd114-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="dd114-109">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP é de 75% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="dd114-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dd114-110">A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.</span><span class="sxs-lookup"><span data-stu-id="dd114-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dd114-111">Uma palavra-chave de Keyword_passport for encontrada.</span><span class="sxs-lookup"><span data-stu-id="dd114-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="dd114-112">Por exemplo, o exemplo a seguir é disparado para a política de **número do Passport US/Reino Unido** : número do Passport 123456789 dos EUA</span><span class="sxs-lookup"><span data-stu-id="dd114-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="dd114-113">Para obter mais informações sobre o que é necessário para que um número de passaporte US/Reino Unido seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram para o número de passaporte US/Reino Unido](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="dd114-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="dd114-114">Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dd114-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  