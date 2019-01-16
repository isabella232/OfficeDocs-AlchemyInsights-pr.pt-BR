---
title: Monitoramento de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275366"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="c14f1-102">Monitoramento de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="c14f1-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="c14f1-p101">Usuários visados com acesso condicional receberá um email de notificação, se elas não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="c14f1-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="c14f1-p102">Se o dispositivo é provável que será registrado, avisa o usuário ir para o aplicativo de Portal da empresa e verifique se ele aparece no Portal de empresa. Caso contrário, o usuário deve registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c14f1-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="c14f1-p103">No portal do Azure, vá para **Intune \> conformidade de dispositivo**. Em **Monitor** , clique em **conformidade do dispositivo**. Exiba o relatório de conformidade do dispositivo para verificar que o dispositivo do usuário está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="c14f1-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="c14f1-p104">No portal do Azure, vá para **Intune \> conformidade de dispositivo**. Em **Gerenciar**, clique em **políticas**. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do usuário. Se nenhum perfil for atribuída, Intune não poderá confirmar o status de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c14f1-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="c14f1-114">Edite a atribuição de condicional de acesso do usuário.</span><span class="sxs-lookup"><span data-stu-id="c14f1-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="c14f1-115">No portal do Azure, vá para **Intune \> acesso condicional \> políticas**</span><span class="sxs-lookup"><span data-stu-id="c14f1-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="c14f1-116">Selecione uma política na lista</span><span class="sxs-lookup"><span data-stu-id="c14f1-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="c14f1-117">Clique em **usuários e grupos**</span><span class="sxs-lookup"><span data-stu-id="c14f1-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="c14f1-p105">Para direcionar a uma determinada política no alguém, adicioná-los à lista de **inclusão** . Para garantir que uma pessoa for omitida da diretiva, adicioná-los à lista de **exclusões** .</span><span class="sxs-lookup"><span data-stu-id="c14f1-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="c14f1-120">Leia mais: [como condicional monitore o acesso de dispositivos](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="c14f1-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

