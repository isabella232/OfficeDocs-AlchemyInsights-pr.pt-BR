---
title: Regra de DLP para SSN que não está funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004970"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas de DLP com Números de Previdência Social

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**Problemas de DLP com SSNs**

Você está com problemas com a Prevenção contra Perda de Dados **(DLP)** não está funcionando para o conteúdo que contém um Número de Segurança **Social (SSN)** ao usar um tipo de informação Microsoft 365? Em caso afirmado, certifique-se de que seu conteúdo contenha as informações necessárias para o que a política de DLP está procurando. 
  
Por exemplo, para uma política SSN configurada com um nível de confiança de 85%, os seguintes são avaliados e devem ser detectados para que a regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 dígitos, que podem estar em um padrão formatado ou não formatado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procurarão SSNs em quatro padrões diferentes:

  - Func_ssn localiza SSNs com formatação forte pré-2011 formatada com traços ou espaços (ddd-dddd OR ddd ddd ddd)

  - Func_unformatted_ssn localiza SSNs com formatação forte pré-2011 que não são formatados como nove dígitos consecutivos (dddddddd)

  - Func_randomized_formatted_ssn localiza SSNs post-2011 que são formatados com traços ou espaços (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn localiza SSNs pós-2011 não formatados como nove dígitos consecutivos (dddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Não, não há Nenhum Checksum

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Uma política de DLP tem 85% de certeza de que detectou esse tipo de informação confidenciais se, dentro de uma proximidade de 300 caracteres:

  - A [função Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) encontra conteúdo que corresponde ao padrão.

  - Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) for encontrada. Exemplos de palavras-chave incluem:  *Previdência Social, Previdência Social#, Soc Sec, SSN*  . Por exemplo, o exemplo a seguir dispararia para a política SSN de DLP: **SSN: 489-36-8350**
  
Para obter mais informações sobre o que é necessário para que os SSNs sejam detectados para seu conteúdo, consulte a seção a seguir neste artigo: O que os Tipos de Informações Confidenciais procurarão [por SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Usando um tipo de informação confidenciais integrado diferente, consulte o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o que os Tipos de Informações [Confidenciais procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  