---
title: Regras de negócios do Dynamics 365 Forms - Regra de Negócios Não Disparar para um Formulário
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947287"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>O evento OnChange não ocorrerá se o campo for alterado programaticamente

O *evento OnChange* não ocorrerá se o campo for alterado programaticamente usando o *atributo.* [método setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se você quiser que os manipuladores de eventos para o *evento OnChange* executem depois de definir o valor, use o método [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) do atributo *formContext.data.entity* em seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
