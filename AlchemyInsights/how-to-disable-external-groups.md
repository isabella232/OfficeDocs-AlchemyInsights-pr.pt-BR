---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457460"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="324dd-102">Como desabilitar grupos externos</span><span class="sxs-lookup"><span data-stu-id="324dd-102">How to disable External Groups</span></span>

<span data-ttu-id="324dd-p101">Mensagens externas aplicam regras de transporte do Exchange (ETRs), um conjunto de controles proativos para impedir que informações empresa sendo compartilhado do Yammer. Para restringir os usuários criem grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configure o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="324dd-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="324dd-105">Depois de ter criado uma regra no Centro de administração do Exchange Online, siga estas etapas para definir ETR a ser aplicado no Yammer:</span><span class="sxs-lookup"><span data-stu-id="324dd-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="324dd-106">Faça logon no Yammer como um administrador verificado e no **Centro de administração no Yammer**, vá para C **onteúdo e segurança \> as configurações de segurança.**</span><span class="sxs-lookup"><span data-stu-id="324dd-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="324dd-107">Em **Mensagens externas**, selecione **impor suas regras de transporte de Exchange Online do Exchange (ETRs) no Yammer.**</span><span class="sxs-lookup"><span data-stu-id="324dd-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="324dd-108">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="324dd-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="324dd-109">Para obter mais informações, consulte [Control externo de mensagens em uma rede do Yammer com regras de transporte do Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="324dd-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

