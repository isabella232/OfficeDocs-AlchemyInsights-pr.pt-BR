---
title: Reprovação de autenticação básica e Exchange PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015677"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="d2faf-102">Reprovação de autenticação básica e Exchange PowerShell</span><span class="sxs-lookup"><span data-stu-id="d2faf-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="d2faf-103">Para obter as informações mais recentes sobre como se conectar ao Exchange Online PowerShell sem o uso da Autenticação Básica, [acesse esse link](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="d2faf-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="d2faf-104">Observe que a Autenticação Básica ainda deve estar habilitada em sua máquina cliente.</span><span class="sxs-lookup"><span data-stu-id="d2faf-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="d2faf-105">O novo módulo do PowerShell v2 usa Autenticação Moderna para estabelecer conexão para habilitar todos os Cmdlets V2 baseados em REST.</span><span class="sxs-lookup"><span data-stu-id="d2faf-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="d2faf-106">Além de cmdlets V2, ela também permite que você acesse Cmdlets mais antigos do PowerShell Remoto (RPS) que exigem que uma sessão do PowerShell Remoto seja estabelecida.</span><span class="sxs-lookup"><span data-stu-id="d2faf-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="d2faf-107">O estabelecimento de uma sessão RPS no computador com Windows exige que o WinRM BasicAuth esteja habilitado no computador cliente, mesmo que o módulo use o mecanismo de Autenticação Moderna para se autenticar no serviço.</span><span class="sxs-lookup"><span data-stu-id="d2faf-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="d2faf-108">O pipeline de Autenticação Básica do WinRM é usado para transportar tokens de Autenticação Moderna.</span><span class="sxs-lookup"><span data-stu-id="d2faf-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="d2faf-109">Se a Autenticação Básica do WinRM estiver desabilitada na máquina cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets mais antigos do RPS não funcionarão).</span><span class="sxs-lookup"><span data-stu-id="d2faf-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
