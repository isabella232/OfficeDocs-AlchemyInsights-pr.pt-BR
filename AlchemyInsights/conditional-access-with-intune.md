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
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662315"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="eacd4-102">Acesso condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="eacd4-102">Conditional Access with Intune</span></span>

<span data-ttu-id="eacd4-103">Usando o **Access condicional** com Intune exige 3 etapas:</span><span class="sxs-lookup"><span data-stu-id="eacd4-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="eacd4-p101">Crie uma **Política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidos para acessar esses recursos. Por exemplo, um dispositivo deve ser compatível com antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="eacd4-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="eacd4-p102">Crie uma **Política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo é considerado compatível. Por exemplo, um dispositivo deve ter um pin de pelo menos 6 dígitos antes que ela é considerada compatível.</span><span class="sxs-lookup"><span data-stu-id="eacd4-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="eacd4-p103">Garantindo a **Políticas de conformidade** e de **Políticas de acesso condicional** são destinadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eacd4-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="eacd4-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="eacd4-110">Read more:</span></span>
  
- [<span data-ttu-id="eacd4-111">Práticas recomendadas de acesso condicionais</span><span class="sxs-lookup"><span data-stu-id="eacd4-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="eacd4-112">Introdução ao Access condicional</span><span class="sxs-lookup"><span data-stu-id="eacd4-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

