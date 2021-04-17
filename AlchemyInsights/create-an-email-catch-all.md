---
title: Criar uma captura de email de todos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816188"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="e257a-102">Criar uma captura de email de todos</span><span class="sxs-lookup"><span data-stu-id="e257a-102">Create an email catch all</span></span>

<span data-ttu-id="e257a-103">O uso de uma captura é fortemente desencorajado.</span><span class="sxs-lookup"><span data-stu-id="e257a-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="e257a-104">É melhor fornecer um retorno para o remetente que permite que os remetentes saibam que sua mensagem não pôde ser entregue como endereçada para que eles possam tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="e257a-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="e257a-105">Você também pode limitar a caixa de correio monitorada para capturar apenas endereços de email anteriormente válidos.</span><span class="sxs-lookup"><span data-stu-id="e257a-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="e257a-106">Qualquer captura de todas as caixas de correio receberá uma boa quantidade de spam e poderá, eventualmente, ser preenchida se não for monitorada de perto.</span><span class="sxs-lookup"><span data-stu-id="e257a-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="e257a-107">(Há limites de recebimento.)</span><span class="sxs-lookup"><span data-stu-id="e257a-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="e257a-108">Se você decidir prosseguir, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="e257a-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="e257a-109">Crie um grupo dinâmico de distribuição & incluir "Todos os tipos de destinatários".</span><span class="sxs-lookup"><span data-stu-id="e257a-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="e257a-110">Crie uma Caixa de Correio dedicada para capturar emails, por exemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="e257a-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="e257a-111">Para o domínio específico, de definir DomainType como "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="e257a-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="e257a-112">Se você remover mais tarde a captura de todos, certifique-se de definir o domínio de volta como Autoritativo.</span><span class="sxs-lookup"><span data-stu-id="e257a-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="e257a-113">Crie uma Regra de Transporte de Fluxo de Email da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="e257a-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="e257a-114">Se o Remetente for "Fora da Organização"</span><span class="sxs-lookup"><span data-stu-id="e257a-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="e257a-115">Redirecionar a mensagem para Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="e257a-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="e257a-116">Exceto se o destinatário for membro do allusers@domain.com (o Grupo de Distribuição contém todos os membros)</span><span class="sxs-lookup"><span data-stu-id="e257a-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="e257a-117">Certifique-se de validar se novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica</span><span class="sxs-lookup"><span data-stu-id="e257a-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
