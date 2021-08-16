---
title: DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030782"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP pode precisar de um tipo personalizado

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**DLP pode exigir um tipo de informação personalizado**

Com uma política de prevenção contra perda de dados (DLP), você pode identificar e proteger dados confidenciais em sua organização. Em alguns cenários, talvez seja necessário criar seu **próprio** tipo personalizado de informações confidenciais para proteger os dados da sua organização.

Por exemplo, sua organização pode precisar identificar e proteger as IDs de funcionários ou outros dados em algum formato específico da sua organização. Em caso afirmado, consulte os artigos a seguir para obter mais informações.
  
 **Personalizar um tipo de informação confidencial interno**
  
Se um tipo de informação confidenciais integrado atender às suas necessidades com apenas alguns ajustes, você poderá personalizar um tipo de informação confidenciais [integrado.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por exemplo, você pode adicionar ou remover palavras-chave ou adicionar ou remover evidências de suporte, como uma data ou endereço.
  
 **Criar um tipo de informação confidencial personalizado**
  
Mas, se você precisar identificar e proteger um tipo [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) diferente de informações confidenciais completamente &, poderá criar um tipo de informação confidenciais personalizado na interface do usuário do Centro de Conformidade e Segurança.
  
**Crie um tipo personalizado de informação confidencial no PowerShell do Centro de Conformidade e Segurança**

Por fim, se a interface do usuário não fornecer todas as opções necessárias, você poderá criar um tipo personalizado de informações confidenciais no Centro de Conformidade e Segurança [& PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ao começar com um arquivo XML, você pode usar todas as opções disponíveis.
