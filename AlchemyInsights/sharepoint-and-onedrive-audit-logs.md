---
title: Relatórios do log de auditoria do SharePoint clássicos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068011"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Logs de auditoria do SharePoint e do OneDrive

**Logs de auditoria de Unificação moderna do SharePoint e do OneDrive da conformidade**

- [Ativar/desativar o log de auditoria unificada](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nenhuma configuração adicional é necessária no SharePoint ou no OneDrive.

- Use a pesquisa de log de auditoria para verificar a atividade do (s) arquivo (s), pasta (s), usuário (s), permissões:

    - [Atividades de arquivo e página](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Atividades de pasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Compartilhamento e acesso às atividades de solicitação](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Atividades de sincronização](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Atividades de administração do site](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Para obter mais informações sobre como recuperar esses eventos, confira [Pesquisar o log de auditoria](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Logs de auditoria clássicos do SharePoint**

Migramos a auditoria herdada do SPO para o log de auditoria unificada (UAL). Essencialmente, isso significa que todos os relatórios de auditoria herdados do SPO serão agora ligados ao UAL, e os sinais de auditoria herdados foram migrados para o UAL.

Principais alterações:

- A remoção de um recurso não está disponível.
- A seção onde você escolhe eventos específicos para auditoria não está disponível. Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.
- A opção "local" em **relatórios personalizados** não está disponível. 
- Eventos de abertura ou download de documentos não estão disponíveis. 

