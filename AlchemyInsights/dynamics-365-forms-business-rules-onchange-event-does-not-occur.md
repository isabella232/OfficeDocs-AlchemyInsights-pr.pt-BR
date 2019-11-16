---
title: Regras comerciais de formulários do Dynamics 365-regra de negócios não está sendo acionada para um formulário
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769327"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>O evento onchange não ocorrerá se o campo for alterado programaticamente

O evento *onChange* não ocorrerá se o campo for alterado programaticamente usando o *atributo.* método [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Se você deseja que manipuladores de eventos para o evento *onChange* sejam executados depois de definir o valor, você deve usar o método *formContext. Data. Entity atributo* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) no seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
