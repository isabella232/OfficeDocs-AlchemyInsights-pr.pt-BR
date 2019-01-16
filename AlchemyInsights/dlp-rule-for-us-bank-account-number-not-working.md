---
title: Regra de DLP para nós número de conta bancária não funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275422"
---
Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo que contém um **Número de conta bancária EUA** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, verifique se seu conteúdo contém as informações necessárias para que a política de DLP está procurando por quando ele é avaliado. 
  
Por exemplo, para uma política de **Número de conta bancária US** configurada com um nível de confiança de 85%, o seguinte é avaliado e deve ser detectado para acionar a regra: 
  
- **[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 17 de 8 dígitos 
    
- **[Padrão:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** dígitos consecutivos de 8-17. 
    
- **[Soma de verificação:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há nenhuma soma de verificação 
    
- **[Definição:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política de DLP é 75% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres: 
    
  - A expressão regular Regex_usa_bank_account_number encontra o conteúdo que corresponde ao padrão
    
  - Uma palavra-chave de Keyword_usa_Bank_Account for encontrada.
    
    Por exemplo, o exemplo a seguir irá disparar para a política de **Número de conta bancária dos Estados Unidos** : conta corrente 78344011 
    
Para obter mais informações sobre o que é necessário para um **Número de conta bancária nos EUA** a serem detectadas para o seu conteúdo, consulte a seção a seguir neste artigo: [O que o confidenciais tipos de informações procure o número de conta bancária dos EUA](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

