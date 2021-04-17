---
title: Pesquisa de Conteúdo Sem Resultados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816836"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="066d2-102">Nenhum resultado da Pesquisa de Conteúdo/Exportações</span><span class="sxs-lookup"><span data-stu-id="066d2-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="066d2-103">Problemas com a Pesquisa de Conteúdo/Exportações que não retornam dados podem ser devido a determinado Filtro de Segurança de Conformidade que foi configurado por um administrador específico e não os comunica a todos os administradores.</span><span class="sxs-lookup"><span data-stu-id="066d2-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="066d2-104">Para resolver isso, verifique se há algum Filtro de Segurança de Conformidade que possa estar causando isso:</span><span class="sxs-lookup"><span data-stu-id="066d2-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="066d2-105">Conectar-se ao Powershell do Centro de Segurança e Conformidade</span><span class="sxs-lookup"><span data-stu-id="066d2-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="066d2-106">Execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="066d2-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="066d2-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="066d2-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="066d2-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="066d2-108">Get-ComplianceSecurityFilter -Organization $org</span></span>