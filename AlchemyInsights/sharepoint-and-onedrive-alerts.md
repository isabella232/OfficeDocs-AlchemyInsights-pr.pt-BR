---
title: Atrasos no recebimento de alertas do SharePoint e do OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563498"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Atrasos no recebimento de alertas do SharePoint e do OneDrive

- Primeiro, verifique a pasta de lixo eletrônico ou spam em seu email.
- Se **todos os alertas de vários arquivos ou bibliotecas estiverem atrasados**, visite o [painel de integridade do serviço](https://portal.office.com/adminportal/home?ref=/servicehealth) para verificar se há avisos/incidentes que possam ocorrer com o SharePoint ou o Exchange. O problema pode ser com o recurso de alerta do SharePoint ou atrasos em emails através do Exchange. Observe também se outros emails estão sendo entregues, caso contrário, o problema é provavelmente com atrasos do Exchange.
- Se **um alerta individual de um arquivo ou biblioteca específico não for entregue**, tente excluí-lo e recriá-lo. Consulte [gerenciar, exibir ou excluir alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.

> [!NOTE]
> - Não é possível enviar alertas para um grupo de distribuição. Só há suporte para grupos de segurança e O365.
> - Você não pode personalizar modelos de email de alerta. Você deve usar o Microsoft Flow ou o fluxo de trabalho do SharePoint Designer para obtê-los.
