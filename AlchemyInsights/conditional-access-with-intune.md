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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504982"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="221d5-102">Acesso condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="221d5-102">Conditional Access with Intune</span></span>

<span data-ttu-id="221d5-103">O uso do **acesso condicional** com o Intune requer três etapas:</span><span class="sxs-lookup"><span data-stu-id="221d5-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="221d5-104">Criar uma **política de acesso condicional** que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="221d5-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="221d5-105">Por exemplo, um dispositivo deve estar em conformidade antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="221d5-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="221d5-106">Crie uma **política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="221d5-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="221d5-107">Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade.</span><span class="sxs-lookup"><span data-stu-id="221d5-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="221d5-108">Garantir que as políticas de **conformidade** e **as políticas de acesso condicional** sejam direcionadas para os grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="221d5-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="221d5-109">Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="221d5-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="221d5-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="221d5-110">Read more:</span></span>
  
- [<span data-ttu-id="221d5-111">Práticas recomendadas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="221d5-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="221d5-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="221d5-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

