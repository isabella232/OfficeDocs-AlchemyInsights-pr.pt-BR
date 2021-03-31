---
title: 126 Não é possível encontrar erro ao obter uma caixa de correio no OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426650"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="7c950-102">Obter uma caixa de correio não encontrada erro no Outlook na Web?</span><span class="sxs-lookup"><span data-stu-id="7c950-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="7c950-103">Se você estiver usando o Outlook na Web e receber uma Caixa de Correio não foi encontrada por erro, **a** conta que você usou para se conectar ao Outlook na Web não tem uma licença do Exchange Online e, portanto, nenhuma caixa de correio está associada à conta.</span><span class="sxs-lookup"><span data-stu-id="7c950-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="7c950-104">O administrador pode atribuir uma licença à sua conta seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="7c950-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="7c950-105">Abra o Centro de administração do  [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para Usuários ativos na seção **Usuários** e selecione o usuário que está vendo o erro.</span><span class="sxs-lookup"><span data-stu-id="7c950-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="7c950-106">Na página de usuário aberta, vá para a seção  Licenças e **Aplicativos,** selecione o valor local apropriado e atribua uma licença que contenha o Exchange Online (expanda a licença para ver seus detalhes).</span><span class="sxs-lookup"><span data-stu-id="7c950-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="7c950-107">Quando terminar, clique em **Salvar alterações**.</span><span class="sxs-lookup"><span data-stu-id="7c950-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="7c950-108">Em alguns casos, se a licença já estiver atribuída a uma conta de usuário, remover e reatribuir a licença ajuda a resolver o problema e a provisioná-la corretamente no sistema:</span><span class="sxs-lookup"><span data-stu-id="7c950-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="7c950-109">Verifique se suas assinaturas do M365 Exchange Online (e outras, se você tiver alguma) estão atuais e não expiraram recentemente.</span><span class="sxs-lookup"><span data-stu-id="7c950-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="7c950-110">Depois de certificar-se de que sua assinatura não expirou e que uma licença válida foi atribuída à conta de usuário, pode levar até 24 horas para que a licença seja provisionada, portanto, talvez seja necessário aguardar a resolução do problema.</span><span class="sxs-lookup"><span data-stu-id="7c950-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="7c950-111">Para obter mais informações, [consulte Atribuir e gerenciar licenças.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="7c950-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>