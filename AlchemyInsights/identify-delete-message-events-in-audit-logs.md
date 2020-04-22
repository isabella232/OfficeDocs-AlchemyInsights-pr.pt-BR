---
title: Identificar eventos de mensagens de exclusão nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716484"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="d6fdb-102">Logs de auditoria para mensagens de email excluídas</span><span class="sxs-lookup"><span data-stu-id="d6fdb-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="d6fdb-103">A partir de janeiro de 2019, a Microsoft está ativando o log de auditoria de caixa de correio por padrão.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="d6fdb-104">Caso contrário, para revisar excluir eventos de mensagem para um usuário específico, você precisará habilitar manualmente as ações de exclusão para auditoria.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="d6fdb-105">Se o log de auditoria de caixa de correio já estiver habilitado para sua organização ou para o usuário específico, siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="d6fdb-106">Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d6fdb-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d6fdb-107">Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d6fdb-108">Selecione o intervalo de datas nos campos **data de início** e data de **término** .</span><span class="sxs-lookup"><span data-stu-id="d6fdb-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d6fdb-109">Especifique o nome de usuário para o usuário que você deseja investigar (o usuário que excluiu os itens).</span><span class="sxs-lookup"><span data-stu-id="d6fdb-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="d6fdb-110">No campo **atividades** , selecione **mensagens excluídas da pasta itens excluídos** e **mensagens movidas para a pasta itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="d6fdb-111">Clique em **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-111">Click **Search**.</span></span>

<span data-ttu-id="d6fdb-112">Nos resultados, selecione um registro de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-112">In the results, select an audit record.</span></span> <span data-ttu-id="d6fdb-113">No submenu detalhes, clique em **mais informações**.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d6fdb-114">Informações adicionais sobre o item excluído (por exemplo, a linha de assunto e o local do item quando ele foi excluído) são exibidas no campo **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="d6fdb-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="d6fdb-115">A propriedade **ClientInfoString** mostrará se a exclusão ocorreu no Outlook, no Outlook na Web (anteriormente conhecido como Outlook Web App) ou em qualquer outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="d6fdb-116">Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="d6fdb-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="d6fdb-117">**Observação**: não é possível recuperar itens excluídos usando o recurso de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d6fdb-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="d6fdb-118">Para recuperar mensagens excluídas no Outlook na Web, confira [recuperar itens excluídos no Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="d6fdb-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
