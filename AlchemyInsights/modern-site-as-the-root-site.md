---
title: Site moderno como o site raiz
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057667"
---
# <a name="modern-site-as-root-site"></a>Site moderno como site raiz

Os clientes de [lançamento de destino](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) agora podem habilitar a experiência de site de comunicação moderna no site raiz clássico do locatário do SharePoint.

Esse recurso pode ser ativado executando um cmdlet simples do PowerShell. Na execução bem-sucedida dos comandos do PowerShell, o site raiz terá uma nova home page do site de comunicação. Os detalhes sobre o cmdlet do PowerShell e os requisitos de recursos estão disponíveis no artigo [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Vamos reverter isso, por padrão, para clientes de lançamento direcionado no início de maio de 2019, e a implantação estará disponível em todo o mundo no final de 2019 de junho. Continue referindo-se ao [centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) para outros novos recursos com o moderno. 

**Importante**: não exclua o site da raiz clássica para criar um site de comunicação moderno. Isso não é suportado pela Microsoft. A exclusão do site raiz tornará todos os sites do SharePoint em sua organização inacessíveis a todos os usuários, até que você restaure o site ou crie um novo site na mesma URL. 
 
 