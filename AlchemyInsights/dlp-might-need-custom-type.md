---
title: A DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932646"
---
# <a name="dlp-might-need-a-custom-type"></a>A DLP pode precisar de um tipo personalizado

**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano. Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup. Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.

Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana. Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período. No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.

**A DLP pode exigir um tipo de informação personalizado**

Com uma política de prevenção de perda de dados (DLP), você pode identificar e proteger dados confidenciais em sua organização. Em alguns cenários, talvez seja necessário criar seu próprio tipo **personalizado** de informações confidenciais para proteger os dados da sua organização.

Por exemplo, sua organização pode precisar identificar e proteger IDs de funcionários ou outros dados em um formato específico para sua organização. Em caso afirmativo, consulte os artigos a seguir para obter mais informações.
  
 **Personalizar um tipo de informação confidencial interno**
  
Se um tipo de informação confidencial interno atender às suas necessidades com apenas alguns ajustes, você poderá [Personalizar um tipo de informação confidencial interno](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Por exemplo, você pode adicionar ou remover palavras-chave ou adicionar ou remover evidências de suporte, como uma data ou um endereço.
  
 **Criar um tipo de informação confidencial personalizado**
  
Mas se você precisar identificar e proteger um tipo diferente de informações confidenciais, poderá [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na interface do usuário do centro de conformidade de & de segurança.
  
**Crie um tipo personalizado de informação confidencial no PowerShell do Centro de Conformidade e Segurança**

Por fim, se a interface do usuário não fornecer todas as opções necessárias, você poderá [criar um tipo de informação confidencial personalizado no PowerShell do centro de conformidade e segurança &](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). A partir de um arquivo XML, você pode usar todas as opções disponíveis.
