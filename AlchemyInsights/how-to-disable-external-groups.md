---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384813"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="9829c-102">Como desabilitar grupos externos</span><span class="sxs-lookup"><span data-stu-id="9829c-102">How to disable External Groups</span></span>

<span data-ttu-id="9829c-103">A mensagem externa do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que as informações da empresa sejam compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="9829c-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="9829c-104">Para impedir que os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="9829c-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="9829c-105">Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir o ETR a ser aplicado no Yammer:</span><span class="sxs-lookup"><span data-stu-id="9829c-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="9829c-106">Faça logon no Yammer como um administrador verificado e, no **centro de administração do Yammer**, vá para **configurações de segurança \> de conteúdo e segurança** de C.</span><span class="sxs-lookup"><span data-stu-id="9829c-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="9829c-107">Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online do Exchange (ETRs) no Yammer.**</span><span class="sxs-lookup"><span data-stu-id="9829c-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="9829c-108">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="9829c-108">Choose **Save**.</span></span>

<span data-ttu-id="9829c-109">Para obter mais informações, consulte [controlar mensagens externas em uma rede do Yammer com regras de transporte do Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="9829c-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  