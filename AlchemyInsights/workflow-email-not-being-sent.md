---
title: O email do fluxo de trabalho não está sendo enviado
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059592"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="0b95d-102">O email do fluxo de trabalho não está sendo enviado</span><span class="sxs-lookup"><span data-stu-id="0b95d-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="0b95d-103">O email de fluxos de trabalho não é enviado a todos os usuários ou apenas usuários específicos, ou você vê o erro **a mensagem de email não pode ser enviada. Certifique-se de que o email tem um destinatário válido**.</span><span class="sxs-lookup"><span data-stu-id="0b95d-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="0b95d-104">Verifique se o usuário existe no grupo de permissões **todas as pessoas** (lista de informações do usuário) para esse conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="0b95d-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="0b95d-105">URL direta de exemplo:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="0b95d-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="0b95d-106">Se o usuário não existir, certifique-se de que o usuário está conectado à página.</span><span class="sxs-lookup"><span data-stu-id="0b95d-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="0b95d-107">Se for um usuário externo, certifique-se de que seu convite tenha sido aceito.</span><span class="sxs-lookup"><span data-stu-id="0b95d-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="0b95d-108">Se o usuário existir no grupo permissões, certifique-se de que o endereço de email está correto.</span><span class="sxs-lookup"><span data-stu-id="0b95d-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="0b95d-109">Se o endereço de email dos usuários não estiver definido aqui, crie um alerta de exemplo para esse usuário que force a sincronização dessa conta de usuário dos perfis de usuário do SharePoint para este conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="0b95d-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="0b95d-110">Os emails de fluxos de trabalho são enviados para os administradores do conjunto de sites, mas não para outros usuários e confira o erro \*\*http proibido para <spam> <spam>. \*\* <spam> <spam></span><span class="sxs-lookup"><span data-stu-id="0b95d-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="0b95d-111">Consulte [acesso negado quando enviado email para grupos](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="0b95d-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="0b95d-112">Além disso, verifique se o recurso de conjunto de sites do **modo de bloqueio de permissão de usuário de acesso limitado** não está ativo.</span><span class="sxs-lookup"><span data-stu-id="0b95d-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="0b95d-113">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="0b95d-113">Related topics</span></span>
- [<span data-ttu-id="0b95d-114">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="0b95d-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0b95d-115">SharePoint e fluxo</span><span class="sxs-lookup"><span data-stu-id="0b95d-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


