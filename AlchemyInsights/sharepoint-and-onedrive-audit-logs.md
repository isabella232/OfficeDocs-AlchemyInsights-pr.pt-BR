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
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="88663-102">Logs de auditoria do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="88663-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="88663-103">**Logs de auditoria de Unificação moderna do SharePoint e do OneDrive da conformidade**</span><span class="sxs-lookup"><span data-stu-id="88663-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="88663-104">Ativar/desativar o log de auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="88663-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="88663-105">Nenhuma configuração adicional é necessária no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="88663-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="88663-106">Use a pesquisa de log de auditoria para verificar a atividade do (s) arquivo (s), pasta (s), usuário (s), permissões:</span><span class="sxs-lookup"><span data-stu-id="88663-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="88663-107">Atividades de arquivo e página</span><span class="sxs-lookup"><span data-stu-id="88663-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="88663-108">Atividades de pasta</span><span class="sxs-lookup"><span data-stu-id="88663-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="88663-109">Compartilhamento e acesso às atividades de solicitação</span><span class="sxs-lookup"><span data-stu-id="88663-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="88663-110">Atividades de sincronização</span><span class="sxs-lookup"><span data-stu-id="88663-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="88663-111">Atividades de administração do site</span><span class="sxs-lookup"><span data-stu-id="88663-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="88663-112">Para obter mais informações sobre como recuperar esses eventos, confira [Pesquisar o log de auditoria](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="88663-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="88663-113">**Logs de auditoria clássicos do SharePoint**</span><span class="sxs-lookup"><span data-stu-id="88663-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="88663-114">Migramos a auditoria herdada do SPO para o log de auditoria unificada (UAL).</span><span class="sxs-lookup"><span data-stu-id="88663-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="88663-115">Essencialmente, isso significa que todos os relatórios de auditoria herdados do SPO serão agora ligados ao UAL, e os sinais de auditoria herdados foram migrados para o UAL.</span><span class="sxs-lookup"><span data-stu-id="88663-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="88663-116">Principais alterações:</span><span class="sxs-lookup"><span data-stu-id="88663-116">Key changes:</span></span>

- <span data-ttu-id="88663-117">A remoção de um recurso não está disponível.</span><span class="sxs-lookup"><span data-stu-id="88663-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="88663-118">A seção onde você escolhe eventos específicos para auditoria não está disponível.</span><span class="sxs-lookup"><span data-stu-id="88663-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="88663-119">Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="88663-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="88663-120">A opção "local" em **relatórios personalizados** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="88663-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="88663-121">Eventos de abertura ou download de documentos não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="88663-121">“Opening or downloading documents” events is NOT available.</span></span> 

