---
title: O fluxo de trabalho não está sendo iniciado
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557957"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está sendo iniciado

- Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão sendo iniciados.

    - Se o seu fluxo de trabalho não estiver sendo iniciado, pode haver um problema de serviço temporário no qual os usuários podem enfrentar atrasos intermitentes com o progresso do fluxo de trabalho. Verifique o [painel de integridade do serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.

    - Se passar mais de 24 horas desde que você viu o problema pela primeira vez, registre um tíquete de suporte. Em muitos casos, já estamos trabalhando em uma solução. Aguarde pelo menos 24 horas para concluir uma solução.

- Fluxos de trabalho do SharePoint 2010 atrasados no início.

    - Isso ocorre se o fluxo de trabalho é acionado em lotes grandes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Os fluxos de trabalho não são projetados para executar em tempo real, de forma que um atraso é o comportamento de design.

   -  Se o fluxo de trabalho é um XMOL (Extensible Object Markup Language) complexo, a compilação pode ser lenta. Confira [este](https://support.microsoft.com/en-us/kb/3043697) artigo.

    - Você deve simplificar o fluxo de trabalho ou recriá-lo usando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.

    - Se o histórico do seu fluxo de trabalho tiver crescido grande, talvez você queira limpar os itens ou criar uma nova lista de histórico.

        Mais informações: [Limpar histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Deseja experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e fluxo](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


