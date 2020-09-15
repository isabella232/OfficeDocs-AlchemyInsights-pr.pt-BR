---
title: 126 não é possível encontrar um erro ao obter uma caixa de correio no OWA?
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
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706738"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="acdbe-102">Obter um erro de caixa de correio não encontrada no Outlook na Web?</span><span class="sxs-lookup"><span data-stu-id="acdbe-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="acdbe-103">Se você estiver usando o Outlook na Web e **não foi possível encontrar uma caixa de correio para** o erro, a conta que você usou para se conectar ao Outlook na Web não tem uma licença do Exchange Online e, portanto, nenhuma caixa de correio está associada à conta.</span><span class="sxs-lookup"><span data-stu-id="acdbe-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="acdbe-104">O administrador pode atribuir uma licença à sua conta, seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="acdbe-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="acdbe-105">Abra o [centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para **usuários ativos** na seção **usuários** e selecione o usuário que está vendo o erro.</span><span class="sxs-lookup"><span data-stu-id="acdbe-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="acdbe-106">Na página do usuário que é aberta, vá para a seção **licenças e aplicativos** , selecione o valor de **local** apropriado e atribua uma licença que contenha o Exchange Online (expanda a licença para ver seus detalhes).</span><span class="sxs-lookup"><span data-stu-id="acdbe-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="acdbe-107">Quando terminar, clique em **Salvar alterações**.</span><span class="sxs-lookup"><span data-stu-id="acdbe-107">When you're finished, click **Save changes**.</span></span>
