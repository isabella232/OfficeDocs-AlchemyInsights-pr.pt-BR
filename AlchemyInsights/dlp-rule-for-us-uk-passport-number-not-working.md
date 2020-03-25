---
title: Regra de DLP para o número do Passport US/Reino Unido que não está funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931250"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com os números de passaporte do DLP-US/Reino Unido

**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano. Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup. Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.

Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana. Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período. No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.

**Problemas de DLP com números do Passport EUA/Reino Unido**

Você está tendo problemas com a **prevenção de perda de dados (DLP)** que não está funcionando para conteúdo que contém um **número de passaporte US/Reino Unido** ao usar um tipo de informação confidencial de DLP no O365? Em caso afirmativo, certifique-se de que o conteúdo contém as informações necessárias para o que a política de DLP está procurando quando é avaliada.
  
Por exemplo, para uma política de **número de passaporte US/Reino Unido** configurada com um nível de confiança de 75%, as seguintes são avaliadas e devem ser detectadas para que a regra seja disparada
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos

- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há checksum

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP é de 75% de certeza de que ela detectou este tipo de informação confidencial se, dentro de uma proximidade de 300 caracteres:

  - A função Func_usa_uk_passport localiza conteúdo que corresponde ao padrão.

  - Uma palavra-chave de Keyword_passport for encontrada.

    Por exemplo, o exemplo a seguir é disparado para a política de **número do Passport US/Reino Unido** : número do Passport 123456789 dos EUA

Para obter mais informações sobre o que é necessário para que um número de passaporte US/Reino Unido seja detectado para seu conteúdo, consulte a seção a seguir neste artigo: o [que os tipos de informações confidenciais procuram para o número de passaporte US/Reino Unido](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Usando um tipo de informação confidencial interno diferente, confira o artigo a seguir para obter informações sobre o que é necessário para outros tipos: o [que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  