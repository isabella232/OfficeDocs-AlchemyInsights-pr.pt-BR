---
title: Acesso condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457442"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c20eb-102">Acesso condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="c20eb-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c20eb-103">Usando o **Access condicional** com Intune exige 3 etapas:</span><span class="sxs-lookup"><span data-stu-id="c20eb-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c20eb-p101">Crie uma **Política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidos para acessar esses recursos. Por exemplo, um dispositivo deve ser compatível com antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="c20eb-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c20eb-p102">Crie uma **Política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo é considerado compatível. Por exemplo, um dispositivo deve ter um pin de pelo menos 6 dígitos antes que ela é considerada compatível.</span><span class="sxs-lookup"><span data-stu-id="c20eb-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c20eb-p103">Garantindo a **Políticas de conformidade** e de **Políticas de acesso condicional** são destinadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c20eb-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c20eb-110">Leia mais</span><span class="sxs-lookup"><span data-stu-id="c20eb-110">Read more:</span></span>
  
- [<span data-ttu-id="c20eb-111">Práticas recomendadas de acesso condicionais</span><span class="sxs-lookup"><span data-stu-id="c20eb-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c20eb-112">Introdução ao Access condicional</span><span class="sxs-lookup"><span data-stu-id="c20eb-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

