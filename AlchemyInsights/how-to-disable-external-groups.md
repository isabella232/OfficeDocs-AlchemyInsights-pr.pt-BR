---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399579"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="05cdd-102">Como desabilitar grupos externos</span><span class="sxs-lookup"><span data-stu-id="05cdd-102">How to disable External Groups</span></span>

<span data-ttu-id="05cdd-103">A mensagem externa do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que as informações da empresa sejam compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="05cdd-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="05cdd-104">Para impedir que os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="05cdd-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="05cdd-105">Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir o ETR a ser aplicado no Yammer:</span><span class="sxs-lookup"><span data-stu-id="05cdd-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="05cdd-106">Faça logon no Yammer como um administrador verificado e, no **centro de administração do Yammer**, vá para C ontenda **e \> configurações de segurança de segurança.**</span><span class="sxs-lookup"><span data-stu-id="05cdd-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="05cdd-107">Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online do Exchange (ETRs) no Yammer.**</span><span class="sxs-lookup"><span data-stu-id="05cdd-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="05cdd-108">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="05cdd-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="05cdd-109">Para obter mais informações, consulte [controlar mensagens externas em uma rede do Yammer com regras de transporte do Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="05cdd-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

