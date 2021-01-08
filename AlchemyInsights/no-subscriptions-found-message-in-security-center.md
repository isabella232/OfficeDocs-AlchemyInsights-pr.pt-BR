---
title: Nenhuma mensagem de assinatura encontrada na Central de Segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768328"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="94c6c-102">Nenhuma mensagem de assinatura encontrada na Central de Segurança</span><span class="sxs-lookup"><span data-stu-id="94c6c-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="94c6c-103">Se, ao acessar a Central de Segurança do Microsoft Defender, você receber uma mensagem "Nenhuma assinatura encontrada", isso significa que o Azure Active Directory (AAD) usado para fazer o logon do usuário no portal não tem uma licença da Proteção Avançada contra Ameaças do Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="94c6c-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="94c6c-104">As licenças do Windows E5 e do Office E5 são licenças separadas.</span><span class="sxs-lookup"><span data-stu-id="94c6c-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="94c6c-105">Abra um caso de suporte se a licença foi adquirida, mas não provisionada para esta instância do AAD.</span><span class="sxs-lookup"><span data-stu-id="94c6c-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="94c6c-106">Ou você tem:</span><span class="sxs-lookup"><span data-stu-id="94c6c-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="94c6c-107">Um possível problema de provisionamento de licença.</span><span class="sxs-lookup"><span data-stu-id="94c6c-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="94c6c-108">Você inadvertidamente provisionou a licença para um Microsoft AAD diferente daquele usado para autenticação no serviço.</span><span class="sxs-lookup"><span data-stu-id="94c6c-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>