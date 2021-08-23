---
title: Meu aplicativo não está sendo exibido na Governança de Aplicativos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362354"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Meu aplicativo não está sendo exibido na Governança de Aplicativos

Se o aplicativo não estiver sendo exibido na Governança de Aplicativos, verifique o seguinte:

1. Vá para [o Azure AD](https://aad.portal.azure.com/) e encontre a ID do aplicativo para seu aplicativo pesquisando o nome do aplicativo na barra superior na página Visão Geral.

1. Acesse Graph Explorer e pesquise a ID do aplicativo na sua entidade de serviço usando essa consulta e substituindo pela ID do aplicativo <appId> relevante: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Se nenhum resultado for retornado, procure a ID do aplicativo no aplicativo usando essa consulta e substituindo pela ID do aplicativo <appId> relevante: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Se você tiver problemas com a consulta, consulte [Obter suporte](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Para obter mais informações ou informações sobre seus Aplicativos na Governança de Aplicativos, [consulte Saiba mais sobre visibilidade e insights.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Para obter mais informações sobre como exibir seus aplicativos, consulte [Exibir seus aplicativos](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
