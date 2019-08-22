---
title: Monitorar o acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538729"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="cc7c3-102">Monitorar o acesso condicional do Exchange</span><span class="sxs-lookup"><span data-stu-id="cc7c3-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="cc7c3-103">Os usuários direcionados ao acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="cc7c3-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="cc7c3-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="cc7c3-105">Se presumir que o dispositivo esteja inscrito, recomende que o usuário acesse o aplicativo do portal da empresa e verifique se ele aparece no portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="cc7c3-106">Caso contrário, o usuário deverá registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="cc7c3-107">No portal do Azure, vá para a \*\*conformidade de dispositivo do Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="cc7c3-108">Em **monitorar** , clique em **conformidade de dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="cc7c3-109">Exiba o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="cc7c3-110">No portal do Azure, vá para a \*\*conformidade de dispositivo do Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="cc7c3-111">Em **gerenciar**, clique em **políticas**.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="cc7c3-112">Na lista de políticas de conformidade, verifique se um perfil foi atribuído ao dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="cc7c3-113">Se nenhum perfil for atribuído, o Intune não conseguirá confirmar o status de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="cc7c3-114">Edite a atribuição de acesso condicional do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc7c3-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="cc7c3-115">No portal do Azure, vá **para \> as políticas \> de acesso condicional do Intune**</span><span class="sxs-lookup"><span data-stu-id="cc7c3-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="cc7c3-116">Selecionar uma política na lista</span><span class="sxs-lookup"><span data-stu-id="cc7c3-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="cc7c3-117">Clique em **usuários e grupos**</span><span class="sxs-lookup"><span data-stu-id="cc7c3-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="cc7c3-118">Para direcionar uma determinada política em alguém, adicione-a à lista de **inclusões** .</span><span class="sxs-lookup"><span data-stu-id="cc7c3-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="cc7c3-119">Para garantir que uma pessoa seja omitida da política, adicione-a à lista de **exclusão** .</span><span class="sxs-lookup"><span data-stu-id="cc7c3-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="cc7c3-120">Leia mais: [como monitorar dispositivos de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="cc7c3-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

