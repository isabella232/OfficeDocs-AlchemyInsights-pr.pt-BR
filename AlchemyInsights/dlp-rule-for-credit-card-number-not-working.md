---
title: Regra DLP para o número de cartão de crédito que não está funcionando
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005078"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemas de DLP com números de cartão de crédito

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**Problemas de DLP com números de cartão de crédito**

Você está com problemas com a Prevenção contra Perda  de Dados **(DLP)** não está funcionando para conteúdo que contém um Número de Cartão de Crédito ao usar um tipo de informação confidenciais de DLP no O365? Em caso afirmado, certifique-se de que o conteúdo contenha as informações necessárias para disparar a política de DLP quando ele for avaliado. Por exemplo, para uma política de **Cartão** de Crédito configurada com um nível de confiança de 85%, os seguintes são avaliados e devem ser detectados para que a regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 dígitos que podem ser formatados ou não formatados (dddddd) e devem passar no teste luhn.

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Padrão muito complexo e robusto que detecta cartões de todas as principais marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões de presente e cartões de lanchonete.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sim, o luhn checksum

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Uma política de DLP tem 85% de certeza de que detectou esse tipo de informação confidenciais se, dentro de uma proximidade de 300 caracteres:

  - A função Func_credit_card localiza conteúdo que corresponde ao padrão.

  - Uma das seguintes opções for verdadeira:

  - Uma palavra-chave de Keyword_cc_verification for encontrada.

  - Uma palavra-chave de Keyword_cc_name é encontrada

  - A função Func_expiration_date encontra uma data no formato de data à direita.

  - O checksum passa

    Por exemplo, o exemplo a seguir dispararia para uma Política de Número de Cartão de Crédito DLP:

  - Visto: 4485 3647 3952 7352
  
  - Expira: 2/2009

Para obter mais informações sobre o que é necessário para que um Número de Cartão de Crédito seja detectado para seu conteúdo, consulte **a** seção a seguir neste artigo: O que os Tipos de Informações Confidenciais procurarão por Cartão de [Crédito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Usando um tipo de informação confidenciais integrado diferente, consulte o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o que os Tipos de Informações [Confidenciais procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  