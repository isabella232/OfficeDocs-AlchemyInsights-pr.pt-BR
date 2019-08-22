---
title: A regra de DLP para SSN não está funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529835"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas de DLP com números de segurança social

Você está tendo problemas com a **prevenção contra perda de dados (DLP)** que não está funcionando para conteúdo que contém um **número de seguridade social (SSN)** ao usar um tipo de informação confidencial no Office 365? Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para o que a política de DLP está procurando. 
  
Por exemplo, para uma política de SSN configurada com um nível de confiança de 85%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 dígitos, que podem estar em um padrão formatado ou não formatado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram CPFs em quatro padrões diferentes:

  - Func_ssn localiza CPFs com uma formatação forte de 2011 formatada com traços ou espaços (DDD-DD-dddd ou DDD DD dddd)

  - Func_unformatted_ssn localiza o CPFs com uma formatação forte de 2011 que não são formatados como nove dígitos consecutivos (ddddddddd)

  - Func_randomized_formatted_ssn localiza o post-2011 CPFs que são formatados com traços ou espaços (DDD-DD-dddd ou DDD DD dddd)

  - Func_randomized_unformatted_ssn localiza o post-2011 CPFs que não estão formatados como nove dígitos consecutivos (ddddddddd)

- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Não, não há checksum

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Uma política de DLP é de 85% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:

  - A [função Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) localiza conteúdo que corresponde ao padrão.

  - Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) for encontrada. Exemplos de palavras-chave incluem: *Social Security, Social Security #, SOC SEC, ssn* . Por exemplo, o exemplo a seguir é disparado para a política de SSN do SSN: **SSN: 489-36-8350**
  
Para obter mais informações sobre o que é necessário para que o CPFs seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram CPFs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  