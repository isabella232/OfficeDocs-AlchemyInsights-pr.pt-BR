---
title: Relatórios do log de auditoria do SharePoint clássicos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662196"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Logs de auditoria do SharePoint e do OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Logs de auditoria clássicos do SharePoint

SPO auditoria herdada foi migrada para o registro de auditoria unificado (UAL). Todos os relatórios de auditoria herdados do SPO serão agora ligados à UAL, e os sinais de auditoria herdados foram migrados para o UAL.

Principais alterações:

* A filtragem não está disponível como um recurso.
* Escolher eventos específicos a serem auditados não está disponível. Consulte [este documento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.
* A opção de **local** em **relatórios personalizados** não está disponível.
* A opção de **abrir ou baixar documentos** de eventos não está disponível.

[Definir configurações de auditoria para um conjunto de sites](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Logs de auditoria de Unificação moderna do SharePoint e do OneDrive da conformidade

* [Ativar/desativar o log de auditoria unificada](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Nenhuma configuração adicional é necessária no SharePoint ou no OneDrive.

Use a pesquisa de log de auditoria para verificar a atividade do (s) arquivo (s), pasta (s), usuário (s), permissões:

* [Atividades de arquivo e página](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Atividades de pasta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Atividades de compartilhamento e solicitação de acesso](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Atividades de sincronização](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Atividades de administração de site](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Para obter mais informações sobre como recuperar esses eventos, confira [Pesquisar o log de auditoria](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
