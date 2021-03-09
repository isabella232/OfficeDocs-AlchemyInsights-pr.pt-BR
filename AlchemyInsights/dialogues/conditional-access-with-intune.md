---
title: Usando o Acesso Condicional com o Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529174"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="2f1b5-102">Usando o Acesso Condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="2f1b5-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="2f1b5-103">O uso do Acesso Condicional com o Intune requer três etapas:</span><span class="sxs-lookup"><span data-stu-id="2f1b5-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="2f1b5-104">Crie uma Política de Conformidade para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="2f1b5-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="2f1b5-105">Crie uma Política de Acesso Condicional que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos. Por exemplo, um dispositivo deve estar em conformidade antes de acessar emails corporativos.</span><span class="sxs-lookup"><span data-stu-id="2f1b5-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="2f1b5-106">Verifique se as Políticas de Conformidade e as Políticas de Acesso Condicional são direcionadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f1b5-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="2f1b5-107">Leia mais...</span><span class="sxs-lookup"><span data-stu-id="2f1b5-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
