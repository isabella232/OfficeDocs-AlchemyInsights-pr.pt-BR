---
title: A DLP não está funcionando conforme o esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079690"
---
# <a name="dlp-not-working-as-expected"></a>A DLP não está funcionando conforme o esperado

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

 **Configuração de DLP**

Você está com problemas com a Prevenção contra Perda de Dados **(DLP)** Office 365 funcionando como esperado? Nesse caso, certifique-se de que sua política **de DLP** está configurada corretamente e que seus dados contenham o que a **política de DLP** está procurando quando ela está sendo avaliada.
  
As políticas DLP permitem identificar e proteger informações confidenciais em sua organização. Para configurar políticas de DLP, use as informações [aqui](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **O que as políticas de DLP procurar**
  
Ao usar os **tipos de** informações confidenciais internas nos centros de Segurança e Conformidade, as políticas DLP procurarão padrões e elementos específicos ao detectar esses tipos confidenciais.
  
- **Tipos de informações confidenciais integrados**

    Para obter informações sobre os tipos Confidenciais integrados e o que uma política DLP procura ao detectar o tipo Sensitive, consulte: O que os tipos de informações confidenciais [procurarão](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipos de informações confidenciais personalizados**

    Se você estiver tentando criar tipos de informações confidenciais personalizados, use o seguinte artigo para obter informações sobre como criar um tipo personalizado de informação confidenciais: Criar um tipo de informação [personalizado e confidenciais.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testar uma política de DLP**

Para testar seus dados com um tipo de informação confidenciais integrado ou personalizado, use a opção **Tipo** de teste em **Classificações** Tipos de informações  >  **confidenciais.** Para obter mais informações, consulte [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Relatórios**
  
- Obter informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Consulte detalhes específicos do evento com um [Relatório de Incidentes.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
