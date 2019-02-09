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
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786686"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com DLP - US / números de passaporte do Reino Unido

Você está tendo problemas com **Data Loss Prevention (DLP)** não está funcionando para conteúdo contendo um **US / número de passaporte do Reino Unido** ao usar um tipo de informações confidenciais de DLP no O365? Em caso afirmativo, verifique se seu conteúdo contém as informações necessárias para que a política de DLP está procurando por quando ele é avaliado. 
  
Por exemplo, para um **US / número de passaporte do Reino Unido** política configurada com um nível de confiança de 75%, o seguinte é avaliado e devem ser detectado para acionar a regra 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos 
    
- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos 
    
- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há nenhuma soma de verificação 
    
- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP é 75% confiante de que detectou esse tipo de informações confidenciais if, dentro de uma proximidade de 300 caracteres: 
    
  - A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.
    
  - Uma palavra-chave de Keyword_passport for encontrada.
    
    Por exemplo, o exemplo a seguir irá disparar para o **US / número de passaporte do Reino Unido** política: número de passaporte US 123456789 
    
Para obter mais informações sobre o que é necessário para um EUA / número de passaporte do Reino Unido a serem detectadas para seu conteúdo, consulte a seção a seguir neste artigo: [aparência do qual o confidenciais tipos de informações para US / número de passaporte do Reino Unido](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Usando um tipo diferente de informações confidenciais internas, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [o que o confidenciais tipos de informações, procure por](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

