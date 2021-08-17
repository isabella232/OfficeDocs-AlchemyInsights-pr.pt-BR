---
title: O conteúdo não aparece nos resultados SharePoint pesquisa
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081598"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>O conteúdo não aparece nos resultados SharePoint pesquisa

Siga estas etapas de solução de problemas quando o conteúdo esperado não aparecer nos resultados da pesquisa:
  
1. Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa. Siga as etapas em [Mostrar conteúdo em um site em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verifique se a **lista ou** **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa. Siga as etapas em [Mostrar conteúdo de listas ou bibliotecas nos resultados da pesquisa.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Verifique se o layout da página, do documento ou da página personalizada é publicado como uma **versão principal.** Siga a etapa 3 [na Pesquisa não retorna todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifique se o usuário tem **permissões** para exibir o conteúdo. Siga as etapas em [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerenciada, editando uma propriedade gerenciada ou removendo uma propriedade gerenciada, será necessário solicitar um rastreamento e um re indexação. **Re indexe** o conteúdo seguindo as etapas em Solicitar manualmente rastreamento e [re indexação](https://docs.microsoft.com/sharepoint/crawl-site-content)de um site, uma biblioteca ou uma lista . Isso pode demorar um pouco, aguarde 24 horas antes de verificar os resultados novamente.

Para obter mais informações, consulte [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
