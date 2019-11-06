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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992606"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8e723-102">Logs de auditoria do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="8e723-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="8e723-103">Logs de auditoria clássicos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="8e723-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="8e723-104">SPO auditoria herdada foi migrada para o registro de auditoria unificado (UAL).</span><span class="sxs-lookup"><span data-stu-id="8e723-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8e723-105">Todos os relatórios de auditoria herdados do SPO serão agora ligados à UAL, e os sinais de auditoria herdados foram migrados para o UAL.</span><span class="sxs-lookup"><span data-stu-id="8e723-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8e723-106">Principais alterações:</span><span class="sxs-lookup"><span data-stu-id="8e723-106">Key changes:</span></span>

* <span data-ttu-id="8e723-107">A filtragem não está disponível como um recurso.</span><span class="sxs-lookup"><span data-stu-id="8e723-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="8e723-108">Escolher eventos específicos a serem auditados não está disponível.</span><span class="sxs-lookup"><span data-stu-id="8e723-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="8e723-109">Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="8e723-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="8e723-110">A opção de **local** em **relatórios personalizados** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="8e723-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="8e723-111">A opção de **abrir ou baixar documentos** de eventos não está disponível.</span><span class="sxs-lookup"><span data-stu-id="8e723-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="8e723-112">Definir configurações de auditoria para um conjunto de sites</span><span class="sxs-lookup"><span data-stu-id="8e723-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="8e723-113">Logs de auditoria de Unificação moderna do SharePoint e do OneDrive da conformidade</span><span class="sxs-lookup"><span data-stu-id="8e723-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="8e723-114">Ativar/desativar o log de auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="8e723-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8e723-115">Nenhuma configuração adicional é necessária no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8e723-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="8e723-116">Use a pesquisa de log de auditoria para verificar a atividade do (s) arquivo (s), pasta (s), usuário (s), permissões:</span><span class="sxs-lookup"><span data-stu-id="8e723-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="8e723-117">Atividades de arquivo e página</span><span class="sxs-lookup"><span data-stu-id="8e723-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="8e723-118">Atividades de pasta</span><span class="sxs-lookup"><span data-stu-id="8e723-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="8e723-119">Compartilhamento e acesso às atividades de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e723-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="8e723-120">Atividades de sincronização</span><span class="sxs-lookup"><span data-stu-id="8e723-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="8e723-121">Atividades de administração do site</span><span class="sxs-lookup"><span data-stu-id="8e723-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="8e723-122">Para obter mais informações sobre como recuperar esses eventos, confira [Pesquisar o log de auditoria](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="8e723-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
