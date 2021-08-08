---
title: O fluxo de trabalho não está iniciando
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907726"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está iniciando

- SharePoint 2010 e SharePoint fluxos de trabalho 2013 não estão iniciando.

    - Se o fluxo de trabalho não estiver iniciando, pode haver um problema de serviço temporário em que os usuários possam ter atrasos intermitentes com o andamento do fluxo de trabalho. Verifique o [Painel de Saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home/servicehealth) para ver se sua organização está impactada.

    - Se mais de 24 horas se passaram desde que você viu esse problema pela primeira vez, registre um tíquete de suporte. Em muitos casos, já estamos trabalhando em uma solução. Dê-nos pelo menos 24 horas para concluir uma solução.

- SharePoint fluxos de trabalho de 2010 atrasados no início.

    - Isso ocorrerá se o fluxo de trabalho for disparado em lotes grandes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Os fluxos de trabalho não são projetados para ser executados em tempo real, portanto, um atraso é o comportamento de design.

   -  Se o Fluxo de Trabalho for XMOL (Linguagem de Marcação de Objeto Extensível complexo), a compilação poderá ser lenta. Confira [este](https://support.microsoft.com//kb/3043697) artigo.

    - Você deve simplificar o fluxo de trabalho ou reprojetá-lo usando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.

    - Se o histórico do fluxo de trabalho tiver se aumentado, talvez você queira limpar os itens ou criar uma nova lista de histórico.

        Mais informações : [Limpar Histórico do Fluxo de Trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Quer tentar Microsoft Flow no SharePoint Online?
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
