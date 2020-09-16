---
title: Notificações de alerta do SharePoint não entregues
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751231"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Notificações de alerta do SharePoint não entregues

Verifique a pasta de lixo eletrônico em seu email, pois, às vezes, os alertas podem ir para lá.

Determine se **todos os alertas não são entregues** ou se **um alerta individual** de um arquivo ou biblioteca específico não é entregue.

- **Alertas individuais não são entregues**: se um alerta individual de um arquivo ou biblioteca específico não for entregue, você poderá tentar excluí-lo e recriá-lo. Consulte [gerenciar, exibir ou excluir alertas do SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.
- **Todos os alertas não são entregues**: se todos os alertas de vários arquivos ou bibliotecas não forem entregues, visite o [painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer com o SharePoint ou o Exchange. O problema pode ser com o recurso de alerta do SharePoint ou atrasos em emails através do Exchange. Também será importante observar se outros emails estão sendo entregues e, caso contrário, o problema provavelmente ocorrerá com os atrasos do Exchange.

Perguntas frequentes sobre alertas:

- Não é possível enviar alertas para o grupo de distribuição, somente os grupos de segurança e O365 têm suporte.
- Você não pode personalizar modelos de email de alerta; Você precisa usar o fluxo de trabalho do Microsoft FLOW ou SharePoint Designer para obtê-los.

## <a name="related-topics"></a>Tópicos Relacionados

Deseja experimentar o Microsoft Flow no SharePoint Online?

- [Criar fluxo](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint e fluxo](https://flow.microsoft.com//blog/sharepoint-and-flow/)
