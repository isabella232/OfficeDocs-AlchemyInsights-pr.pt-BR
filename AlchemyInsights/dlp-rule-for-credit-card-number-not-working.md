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
Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo que contém um **Número de cartão de crédito** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, certifique-se de seu conteúdo contém as informações necessárias para acionar a política de DLP quando ele é avaliado. Por exemplo, para uma **política de cartão de crédito** configurado com um nível de confiança de 85%, a seguir é avaliadas e deve ser detectadas para acionar a regra: 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatado (dddddddddddddddd) e deve passar o teste de Luhn. 
    
- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Muito complexa e robusto padrão que detecta cartões de todas as principais marcas nível mundiais, incluindo Visa, Mastercard, Discover Card, JCB, American Express, cartões de vale-presente e cartões de cliente. 
    
- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação Luhn 
    
- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política DLP é de 85% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres: 
    
  - A função Func_credit_card localiza conteúdo que corresponde ao padrão.
    
  - Uma das seguintes opções for verdadeira: 
    
  - Uma palavra-chave de Keyword_cc_verification for encontrada.
    
  - Uma palavra-chave da Keyword_cc_name for encontrada
    
  - A função Func_expiration_date encontra uma data no formato de data à direita.
    
  - Passa a soma de verificação
    
    Por exemplo, o exemplo a seguir irá disparar para uma política de número de cartão de crédito DLP:
    
  - Visa: 4485 3647 3952 7352 
    
  - Expira: 2/2009
    
Para obter mais informações sobre o que é necessário para um **Número de cartão de crédito** a serem detectadas para o seu conteúdo, consulte a seção a seguir neste artigo: [O que o confidenciais tipos de informações procure o cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

