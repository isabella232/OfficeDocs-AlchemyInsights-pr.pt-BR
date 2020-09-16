---
title: O email do fluxo de trabalho não está sendo enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748977"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="c395b-102">O email do fluxo de trabalho não está sendo enviado para uma lista ou biblioteca do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c395b-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="c395b-103">Os emails de fluxos de trabalho não são enviados a todos os usuários ou apenas usuários específicos, ou você vê o erro **a mensagem de email não pode ser enviada. Certifique-se de que o email tem um destinatário válido**.</span><span class="sxs-lookup"><span data-stu-id="c395b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="c395b-104">Verifique se o usuário existe no grupo de permissões **todas as pessoas** (lista de informações do usuário) para esse conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="c395b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="c395b-105">URL direta de exemplo: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="c395b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="c395b-106">Se o usuário não existir, certifique-se de que o usuário está conectado à página.</span><span class="sxs-lookup"><span data-stu-id="c395b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="c395b-107">Se for um usuário externo, certifique-se de que seu convite tenha sido aceito.</span><span class="sxs-lookup"><span data-stu-id="c395b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="c395b-108">Se o usuário existir no grupo permissões, certifique-se de que o endereço de email está correto.</span><span class="sxs-lookup"><span data-stu-id="c395b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="c395b-109">Se o endereço de email dos usuários não estiver definido aqui, crie um alerta de exemplo para esse usuário que force a sincronização dessa conta de usuário dos perfis de usuário do SharePoint para este conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="c395b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="c395b-110">Os emails de fluxos de trabalho são enviados para os administradores do conjunto de sites, mas não para outros usuários e confira o erro **http proibido para <span>https:</span>//URL/_vti_bin/Client.XVC.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="c395b-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="c395b-111">Consulte [acesso negado ao enviar um email a um grupo do SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="c395b-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="c395b-112">Além disso, verifique se o recurso de conjunto de sites do **modo de bloqueio de permissão de usuário de acesso limitado** não está ativo.</span><span class="sxs-lookup"><span data-stu-id="c395b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="c395b-113">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="c395b-113">Related topics</span></span>
<span data-ttu-id="c395b-114">Deseja experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="c395b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="c395b-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="c395b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c395b-116">SharePoint e fluxo</span><span class="sxs-lookup"><span data-stu-id="c395b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


