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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544096"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="91493-102">Nenhuma mensagem de assinatura encontrada na Central de Segurança</span><span class="sxs-lookup"><span data-stu-id="91493-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="91493-103">Se, ao acessar a Central de Segurança do Microsoft Defender, você receber uma mensagem "Nenhuma assinatura encontrada", isso significa que o Azure Active Directory (AAD) usado para fazer logon do usuário no portal não tem uma licença do Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="91493-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="91493-104">As licenças do Windows E5 e do Office E5 são licenças separadas.</span><span class="sxs-lookup"><span data-stu-id="91493-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="91493-p101">Abra um caso de suporte se a licença foi adquirida, mas não provisionada para esta instância do AAD. Ou você tem:</span><span class="sxs-lookup"><span data-stu-id="91493-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="91493-107">Um possível problema de provisionamento de licença.</span><span class="sxs-lookup"><span data-stu-id="91493-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="91493-108">Você inadvertidamente provisionou a licença para um Microsoft AAD diferente daquele usado para autenticação no serviço.</span><span class="sxs-lookup"><span data-stu-id="91493-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>