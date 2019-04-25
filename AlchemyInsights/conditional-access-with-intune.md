---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393529"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="07a59-102">Acesso condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="07a59-102">Conditional Access with Intune</span></span>

<span data-ttu-id="07a59-103">O uso do **acesso condicional** com o Intune requer três etapas:</span><span class="sxs-lookup"><span data-stu-id="07a59-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="07a59-104">Criar uma **política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="07a59-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="07a59-105">Por exemplo, um dispositivo deve estar em conformidade antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="07a59-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="07a59-106">Crie uma **política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="07a59-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="07a59-107">Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade.</span><span class="sxs-lookup"><span data-stu-id="07a59-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="07a59-108">Garantir que as políticas de **conformidade** e **as políticas de acesso condicional** sejam direcionadas para os grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="07a59-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="07a59-109">Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="07a59-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="07a59-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="07a59-110">Read more:</span></span>
  
- [<span data-ttu-id="07a59-111">Práticas recomendadas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="07a59-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="07a59-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="07a59-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

