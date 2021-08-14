---
title: Regra de DLP para o número de conta bancária dos EUA que não está funcionando
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005006"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemas de DLP com números de conta bancária dos EUA

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**Problemas de DLP com números de conta bancária dos EUA**

Você está com problemas com a Prevenção contra Perda  de Dados **(DLP)** não está funcionando para conteúdo que contém um número de conta bancária dos EUA ao usar um tipo de informação confidenciais de DLP no O365? Em caso afirmado, certifique-se de que seu conteúdo contenha as informações necessárias para o que a política de DLP está procurando quando avaliada.
  
Por exemplo, para uma política de Número de Conta Bancária dos EUA configurada com um nível de confiança de 85%, os seguintes são avaliados e devem ser detectados para que **a** regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8 a 17 dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 a 17 dígitos consecutivos.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Nenhum Checksum

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Uma política de DLP tem 75% de certeza de que detectou esse tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A expressão regular Regex_usa_bank_account_number encontra conteúdo que corresponde ao padrão

  - Uma palavra-chave de Keyword_usa_Bank_Account for encontrada.

    Por exemplo, o exemplo a seguir dispararia para a **política número** de conta bancária dos EUA: Verificação de 78344011

Para obter mais informações sobre o que é necessário para que um Número de Conta Bancária dos EUA seja detectado para seu conteúdo, consulte **a** seção a seguir neste artigo: O que os Tipos de Informações Confidenciais procurarão por Número de Conta Bancária dos [EUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Usando um tipo de informação confidenciais integrado diferente, consulte o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o que os Tipos de Informações [Confidenciais procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  