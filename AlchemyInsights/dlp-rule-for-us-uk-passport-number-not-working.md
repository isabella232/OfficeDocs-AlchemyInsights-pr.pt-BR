---
title: Regra de DLP para o número do Passport US/Reino Unido que não está funcionando
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679212"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com os números de passaporte do DLP-US/Reino Unido

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**Problemas de DLP com números do Passport EUA/Reino Unido**

Você está tendo problemas com a **prevenção de perda de dados (DLP)** que não está funcionando para conteúdo que contém um **número de passaporte US/Reino Unido** ao usar um tipo de informação confidencial de DLP no O365? Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para o que a política de DLP está procurando quando é avaliada.
  
Por exemplo, para uma política de **número de passaporte US/Reino Unido** configurada com um nível de confiança de 75%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove dígitos consecutivos

- **[Soma de verificação:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há checksum

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Uma política de DLP é de 75% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:

  - A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.

  - Uma palavra-chave de Keyword_passport for encontrada.

    Por exemplo, o exemplo a seguir é disparado para a política de **número do Passport US/Reino Unido** : número do Passport 123456789 dos EUA

Para obter mais informações sobre o que é necessário para que um número de passaporte US/Reino Unido seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram para o número de passaporte US/Reino Unido](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  