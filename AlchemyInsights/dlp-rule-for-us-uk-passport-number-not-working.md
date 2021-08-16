---
title: Regra de DLP para o Número de Passaporte dos EUA/Reino Unido que não está funcionando
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004934"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com DLP - números de passaporte dos EUA/Reino Unido

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**Problemas de DLP com números de passaporte dos EUA/Reino Unido**

Você está com problemas com a Prevenção contra Perda de Dados **(DLP)** não está funcionando para conteúdo que contém um número de passaporte dos **EUA/Reino** Unido ao usar um tipo de informação confidenciais de DLP no O365? Em caso afirmado, certifique-se de que seu conteúdo contenha as informações necessárias para o que a política de DLP está procurando quando avaliada.
  
Por exemplo, para uma política de número de passaporte dos **EUA/Reino** Unido configurada com um nível de confiança de 75%, os seguintes são avaliados e devem ser detectados para que a regra seja disparada
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove dígitos consecutivos

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Nenhum Checksum

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Uma política de DLP tem 75% de certeza de que detectou esse tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.

  - Uma palavra-chave de Keyword_passport for encontrada.

    Por exemplo, o exemplo a seguir dispararia para a política de número de passaporte dos **EUA/Reino** Unido: número de passaporte dos EUA 123456789

Para obter mais informações sobre o que é necessário para que um Número de Passaporte dos EUA/Reino Unido seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: O que os Tipos de Informações Confidenciais procurarão por Número de Passaporte dos [EUA/Reino Unido](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Usando um tipo de informação confidenciais integrado diferente, consulte o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o que os Tipos de Informações [Confidenciais procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  