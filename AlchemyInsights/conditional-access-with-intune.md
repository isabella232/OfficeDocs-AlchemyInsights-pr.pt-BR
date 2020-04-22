---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706009"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="df378-102">Acesso condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="df378-102">Conditional Access with Intune</span></span>

<span data-ttu-id="df378-103">O uso do **acesso condicional** com o Intune requer três etapas:</span><span class="sxs-lookup"><span data-stu-id="df378-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="df378-104">Criar uma **política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="df378-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="df378-105">Por exemplo, um dispositivo deve estar em conformidade antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="df378-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="df378-106">Crie uma **política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="df378-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="df378-107">Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade.</span><span class="sxs-lookup"><span data-stu-id="df378-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="df378-108">Garantir que as políticas de **conformidade** e **as políticas de acesso condicional** sejam direcionadas para os grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="df378-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="df378-109">Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="df378-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="df378-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="df378-110">Read more:</span></span>
  
- [<span data-ttu-id="df378-111">Práticas recomendadas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="df378-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="df378-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="df378-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

