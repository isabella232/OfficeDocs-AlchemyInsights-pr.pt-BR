---
title: DLP não está funcionando conforme esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977426"
---
# <a name="dlp-not-working-as-expected"></a>DLP não está funcionando conforme esperado

**Importante**: durante esses horários sem precedentes, estamos executando etapas para garantir que o SharePoint Online e os serviços do onedrive permaneçam altamente disponíveis – visite [ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

 **Configurando DLP**

Você está tendo problemas com a **prevenção de perda de dados (DLP)** no Office 365 que não está funcionando conforme o esperado? Em caso afirmativo, certifique-se de que sua **política de DLP** está configurada corretamente e que seus dados contêm o que a **política de DLP** está procurando quando estiver sendo avaliada.
  
As políticas de DLP permitem identificar e proteger informações confidenciais em sua organização. Para configurar as políticas de DLP, use as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **O que as políticas de DLP procuram**
  
Ao usar os **tipos de informações confidenciais internas** no centro de segurança e conformidade do Office 365, as políticas de DLP procuram padrões e elementos específicos ao detectar esses tipos confidenciais.
  
- **Tipos de informações confidenciais internas**

    Para obter informações sobre os tipos confidenciais internos e o que a política de DLP procura ao detectar o tipo confidencial, consulte: [o que os tipos de informações confidenciais procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Tipos de informações confidenciais personalizadas**

    Se você estiver tentando criar tipos de informações confidenciais personalizados, use o artigo a seguir para obter informações sobre como criar um tipo confidencial personalizado: [criar um tipo de informação confidencial personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testar uma política de DLP**

Para testar seus dados com um tipo de informação confidencial interno ou personalizado, use a opção **tipo de teste** em **classificações** > **confidenciais tipos de informações**. Para obter mais informações, consulte [testar tipos de informações confidenciais personalizados](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Relatórios**
  
- Obtenha informações confidenciais sobre os relatórios de [DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Veja detalhes específicos do evento com um [relatório de incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
