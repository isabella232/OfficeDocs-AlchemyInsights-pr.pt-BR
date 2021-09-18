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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446679"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP pode precisar de um tipo personalizado

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**DLP pode exigir um tipo de informação personalizado**

Com uma política de prevenção contra perda de dados (DLP), você pode identificar e proteger dados confidenciais em sua organização. Em alguns cenários, talvez seja necessário criar seu próprio tipo personalizado de informações confidenciais para proteger os dados da sua organização. Para obter mais informações, [consulte Learn about sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) and Sensitive information type entity [definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Para obter mais informações sobre como criar tipos e políticas de informações confidenciais personalizados, consulte: 

**Personalizar um tipo de informação confidencial interno**

Se um tipo de informação confidenciais integrado atender às suas necessidades com apenas alguns ajustes, consulte Personalizar um tipo de informação [confidenciais integrado.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por exemplo, você pode adicionar ou remover palavras-chave ou adicionar ou remover evidências de suporte, como uma data ou endereço.

**Criar um tipo de informação confidencial personalizado**

Mas, se você precisar identificar e proteger um tipo diferente de informações confidenciais completamente, poderá criar um tipo de informação confidenciais personalizado no Centro de conformidade do Microsoft 365. Para obter mais informações, [consulte Get started with custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Crie um tipo personalizado de informação confidencial no PowerShell do Centro de Conformidade e Segurança**

Por fim, se a interface do usuário não fornecer todas as opções necessárias, você poderá criar um tipo de informação confidenciais personalizado no Centro de Conformidade e Segurança & do PowerShell. Ao começar com um arquivo XML, você pode usar todas as opções disponíveis. Para obter mais informações, [consulte Create a custom sensitive information type using PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Para testar sua política primeiro no modo de teste, consulte [Implement policy in test mode](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) e [Create, test, and tune a DLP policy](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 