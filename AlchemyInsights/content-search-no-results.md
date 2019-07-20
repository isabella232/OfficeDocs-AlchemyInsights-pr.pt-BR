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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800170"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="e6fb7-102">Nenhum resultado de pesquisa/exportação de conteúdo</span><span class="sxs-lookup"><span data-stu-id="e6fb7-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="e6fb7-103">Problemas de pesquisa/exportação de conteúdo que não retornam dados podem ser devido ao certo filtro de segurança de conformidade que foi configurado por um administrador específico e não está se comunicando com todos os administradores.</span><span class="sxs-lookup"><span data-stu-id="e6fb7-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="e6fb7-104">Para resolver isso, verifique se há algum filtro de segurança de conformidade que possa estar causando o seguinte:</span><span class="sxs-lookup"><span data-stu-id="e6fb7-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="e6fb7-105">Conectar-se ao PowerShell do centro de conformidade e segurança</span><span class="sxs-lookup"><span data-stu-id="e6fb7-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e6fb7-106">Execute o seguinte comandos:</span><span class="sxs-lookup"><span data-stu-id="e6fb7-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="e6fb7-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="e6fb7-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="e6fb7-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="e6fb7-108">Get-ComplianceSecurityFilter -Organization $org</span></span>