---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750544"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

Se um site do OneDrive ou do SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário. [Verifique o painel de integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).

**Adicionar e licenciar o usuário**

Certifique-se de [atribuir licenças aos usuários no Office 365 para empresas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Atribuir permissões**

Se o usuário tiver recebido uma licença do SharePoint e ainda estiver recebendo uma mensagem de acesso negado, verifique se ele tem o [nível de permissão apropriado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.

**Considere usar o recurso de solicitação de acesso**

O [recurso de solicitação de acesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite que as pessoas solicitem acesso ao conteúdo que eles não têm permissão para ver no momento.

**Permitir que o script personalizado possa causar problemas de acesso negado**

Há determinados cenários em que o recurso *permitir script personalizado* pode estar apresentando um acesso negado. Para obter uma lista dos recursos afetados, considerações sobre segurança e a capacidade de desabilitar o recurso. Visite [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

