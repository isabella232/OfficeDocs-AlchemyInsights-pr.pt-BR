---
title: Criar um email capturar tudo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712974"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="32184-102">Criar um email capturar tudo</span><span class="sxs-lookup"><span data-stu-id="32184-102">Create an email catch all</span></span>

<span data-ttu-id="32184-103">O uso de um catch tudo é fortemente desencorajado.</span><span class="sxs-lookup"><span data-stu-id="32184-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="32184-104">É melhor fornecer um repercussão para o remetente, permitindo que os remetentes saibam que a mensagem não puderam ser entregues conforme tratados, para que eles possam realizar ações.</span><span class="sxs-lookup"><span data-stu-id="32184-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="32184-105">Você também pode limitar a caixa de correio monitorada para capturar apenas endereços de email válidos.</span><span class="sxs-lookup"><span data-stu-id="32184-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="32184-106">Qualquer caixa de correio do catch receberá uma boa dose de spam e poderá, eventualmente, preencher se não estiver intimamente monitorado.</span><span class="sxs-lookup"><span data-stu-id="32184-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="32184-107">(Há limites de recebimento.)</span><span class="sxs-lookup"><span data-stu-id="32184-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="32184-108">Se você decidir continuar, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="32184-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="32184-109">Criar um grupo dinâmico de distribuição & incluir "todos os tipos de destinatário."</span><span class="sxs-lookup"><span data-stu-id="32184-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="32184-110">Criar uma caixa de correio dedicada para capturar emails, por exemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="32184-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="32184-111">Para o domínio específico, defina o DomainType como "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="32184-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="32184-112">Se posteriormente você remover o catch, certifique-se de definir o domínio novamente como autoritativo.</span><span class="sxs-lookup"><span data-stu-id="32184-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="32184-113">Crie uma regra de transporte fluxo da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="32184-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="32184-114">Se o remetente for "fora da organização"</span><span class="sxs-lookup"><span data-stu-id="32184-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="32184-115">Redirecionar a mensagem para o Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="32184-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="32184-116">Exceto se o destinatário for um membro de allusers@domain.com (grupo de distribuição contém todos os membros)</span><span class="sxs-lookup"><span data-stu-id="32184-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="32184-117">Certifique-se de validar que novas caixas de correio são adicionadas ao grupo dinâmico de distribuição</span><span class="sxs-lookup"><span data-stu-id="32184-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
