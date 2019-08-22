---
title: Pesquisa de conteúdo sem resultados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516767"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="d75f6-102">Nenhum resultado de pesquisa/exportação de conteúdo</span><span class="sxs-lookup"><span data-stu-id="d75f6-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="d75f6-103">Problemas de pesquisa/exportação de conteúdo que não retornam dados podem ser devido ao certo filtro de segurança de conformidade que foi configurado por um administrador específico e não está se comunicando com todos os administradores.</span><span class="sxs-lookup"><span data-stu-id="d75f6-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="d75f6-104">Para resolver isso, verifique se há algum filtro de segurança de conformidade que possa estar causando o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d75f6-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="d75f6-105">Conectar-se ao PowerShell do centro de conformidade e segurança</span><span class="sxs-lookup"><span data-stu-id="d75f6-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="d75f6-106">Execute o seguinte comandos:</span><span class="sxs-lookup"><span data-stu-id="d75f6-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="d75f6-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="d75f6-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="d75f6-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="d75f6-108">Get-ComplianceSecurityFilter -Organization $org</span></span>