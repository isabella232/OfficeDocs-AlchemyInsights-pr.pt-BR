---
title: Local dos dados
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627834"
---
# <a name="data-location"></a>Local dos dados

Você pode exibir o local do seu locatário do Office 365 no centro de administração ou conectando-se ao Exchange Online por meio do PowerShell.


**Centro de administração:**
1. Faça logon no [centro de administração](https://admin.microsoft.com/Adminportal/Home).
2. Selecione **configurações** > **perfil da organização**.
3. Em **local dos dados**, selecione **Exibir detalhes**.


**™**
1. Conecte-se ao Exchange Online usando o Windows PowerShell.
2. Execute o cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) para exibir uma lista das propriedades do locatário. 
3. Observe a propriedade OrganizationId.

Quando você tem o local de dados do EXO e do SPO, é possível determinar o local dos dados de outros serviços que você pode usar de [onde seus dados estão localizados](https://products.office.com/where-is-your-data-located).