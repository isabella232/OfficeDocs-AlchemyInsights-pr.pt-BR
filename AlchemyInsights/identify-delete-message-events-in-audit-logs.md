---
title: Identificar eventos de mensagens de exclusão nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755141"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="bf43a-102">Logs de auditoria para mensagens de email excluídas</span><span class="sxs-lookup"><span data-stu-id="bf43a-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="bf43a-103">A partir de janeiro de 2019, a Microsoft está ativando o log de auditoria de caixa de correio por padrão.</span><span class="sxs-lookup"><span data-stu-id="bf43a-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="bf43a-104">Caso contrário, para revisar excluir eventos de mensagem para um usuário específico, você precisará habilitar manualmente as ações de exclusão para auditoria.</span><span class="sxs-lookup"><span data-stu-id="bf43a-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="bf43a-105">Se o log de auditoria de caixa de correio já estiver habilitado para sua organização ou para o usuário específico, siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="bf43a-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="bf43a-106">Faça logon no [centro de conformidade & segurança do Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="bf43a-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="bf43a-107">Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="bf43a-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="bf43a-108">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="bf43a-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="bf43a-109">Especifique o nome de usuário para o usuário que você deseja investigar (o usuário que excluiu os itens).</span><span class="sxs-lookup"><span data-stu-id="bf43a-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="bf43a-110">No campo **atividades** , selecione **mensagens excluídas da pasta itens excluídos** e **mensagens movidas para a pasta itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="bf43a-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="bf43a-111">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="bf43a-111">Click **Search**.</span></span>

<span data-ttu-id="bf43a-112">Nos resultados, selecione um registro de auditoria.</span><span class="sxs-lookup"><span data-stu-id="bf43a-112">In the results, select an audit record.</span></span> <span data-ttu-id="bf43a-113">No submenu detalhes, clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="bf43a-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="bf43a-114">Informações adicionais sobre o item excluído (por exemplo, a linha de assunto e o local do item quando ele foi excluído) são exibidas no campo **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="bf43a-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="bf43a-115">A propriedade **ClientInfoString** mostrará se a exclusão ocorreu no Outlook, no Outlook na Web (anteriormente conhecido como Outlook Web App) ou em qualquer outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf43a-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="bf43a-116">Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="bf43a-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="bf43a-117">**Observação**: não é possível recuperar itens excluídos usando o recurso de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="bf43a-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="bf43a-118">Para recuperar mensagens excluídas no Outlook na Web, confira [recuperar itens excluídos no Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="bf43a-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
