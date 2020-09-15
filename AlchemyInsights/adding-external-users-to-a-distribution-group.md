---
title: Adicionando usuários externos a um grupo de distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663501"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="7795c-102">Adicionar usuários externos a um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="7795c-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="7795c-103">A adição de um contato externo a um grupo de distribuição (DG) é um processo de duas etapas:</span><span class="sxs-lookup"><span data-stu-id="7795c-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="7795c-104">Criar um contato de email para o usuário externo:</span><span class="sxs-lookup"><span data-stu-id="7795c-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="7795c-105">No centro de administração, vá para a página contatos **dos usuários**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="7795c-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="7795c-106">Selecione **Adicionar um contato**.</span><span class="sxs-lookup"><span data-stu-id="7795c-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="7795c-107">Digite as informações do contato e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="7795c-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="7795c-108">Adicione o contato de email ao seu DG:</span><span class="sxs-lookup"><span data-stu-id="7795c-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="7795c-109">No centro de administração, vá para a página grupos de **grupos**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="7795c-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="7795c-110">Localize o DG ao qual você deseja adicionar o usuário externo e selecione-o para abrir a caixa de diálogo Editar.</span><span class="sxs-lookup"><span data-stu-id="7795c-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="7795c-111">Na guia **Membros** , selecione **Exibir todos e gerenciar Membros**.</span><span class="sxs-lookup"><span data-stu-id="7795c-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="7795c-112">Escolha **Adicionar membros**.</span><span class="sxs-lookup"><span data-stu-id="7795c-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="7795c-113">Selecione o contato de email que você criou na etapa anterior e, em seguida, selecione **salvar**.</span><span class="sxs-lookup"><span data-stu-id="7795c-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="7795c-114">Se após seguir estas etapas, seus usuários externos não podem enviar emails para o DG ou não receber emails dele, pode ser que o DG esteja marcado para permitir apenas emails de usuários internos.</span><span class="sxs-lookup"><span data-stu-id="7795c-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="7795c-115">Você pode verificar essa configuração e corrigi-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="7795c-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="7795c-116">**Observação:** Estas instruções não se aplicam se o tipo de seu grupo for "Microsoft 365 Group" em vez de "grupo de distribuição".</span><span class="sxs-lookup"><span data-stu-id="7795c-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="7795c-117">Se esse for o caso, você poderá adicionar o usuário externo diretamente ao grupo do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7795c-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="7795c-118">Informações detalhadas sobre os convidados de grupos do Microsoft 365, bem como instruções para a adição de convidados externos, podem ser encontradas neste [artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="7795c-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  