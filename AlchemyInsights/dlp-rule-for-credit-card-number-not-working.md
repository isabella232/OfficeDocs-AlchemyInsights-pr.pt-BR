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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529943"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemas de DLP com números de cartão de crédito

Você está tendo problemas com a **prevenção contra perda de dados (DLP)** não está funcionando para conteúdo que contém um **número de cartão de crédito** ao usar um tipo de informação confidencial de DLP no O365? Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para acionar a política de DLP quando for avaliada. Por exemplo, para uma **política de cartão de crédito** configurada com um nível de confiança de 85%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (dddddddddddddddd) e deve passar o teste Luhn.

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Um padrão muito complexo e robusto que detecta cartões de todas as principais marcas em todo o mundo, incluindo Visa, MasterCard, cartão de descoberta, JCB, American Express, Gift e cartões Diner.

- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação Luhn

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP é de 85% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:

  - A função Func_credit_card localiza conteúdo que corresponde ao padrão.

  - Uma das seguintes opções for verdadeira:

  - Uma palavra-chave de Keyword_cc_verification for encontrada.

  - Uma palavra-chave de Keyword_cc_name for encontrada

  - A função Func_expiration_date encontra uma data no formato de data à direita.

  - O checksum passa

    Por exemplo, o exemplo a seguir é disparado para uma política de número de cartão de crédito DLP:

  - Visa: 4485 3647 3952 7352
  
  - Expira em: 2/2009

Para obter mais informações sobre o que é necessário para que um **número de cartão de crédito** seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram por cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  