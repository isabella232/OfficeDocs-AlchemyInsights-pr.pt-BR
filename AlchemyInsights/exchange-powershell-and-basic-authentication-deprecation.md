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
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205183"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="a9f13-102">Reprovação de autenticação básica e Exchange PowerShell</span><span class="sxs-lookup"><span data-stu-id="a9f13-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="a9f13-103">Para obter as informações mais recentes sobre como se conectar ao Exchange Online PowerShell sem o uso da Autenticação Básica, [acesse esse link](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="a9f13-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="a9f13-104">O módulo PowerShell V2 não usa a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="a9f13-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="a9f13-105">Observe que a Autenticação Básica ainda deve estar habilitada em sua máquina cliente.</span><span class="sxs-lookup"><span data-stu-id="a9f13-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="a9f13-106">O novo módulo do PowerShell v2 usa Autenticação Moderna para estabelecer conexão para habilitar todos os Cmdlets V2 baseados em REST.</span><span class="sxs-lookup"><span data-stu-id="a9f13-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="a9f13-107">Além de cmdlets V2, ela também permite que você acesse Cmdlets mais antigos do PowerShell Remoto (RPS) que exigem que uma sessão do PowerShell Remoto seja estabelecida.</span><span class="sxs-lookup"><span data-stu-id="a9f13-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="a9f13-108">O estabelecimento de uma sessão RPS no computador com Windows exige que o WinRM BasicAuth esteja habilitado no computador cliente, mesmo que o módulo use o mecanismo de Autenticação Moderna para se autenticar no serviço.</span><span class="sxs-lookup"><span data-stu-id="a9f13-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="a9f13-109">O pipeline de Autenticação Básica do WinRM é usado para transportar tokens de Autenticação Moderna.</span><span class="sxs-lookup"><span data-stu-id="a9f13-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="a9f13-110">Se a Autenticação Básica do WinRM estiver desabilitada na máquina cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets mais antigos do RPS não funcionarão).</span><span class="sxs-lookup"><span data-stu-id="a9f13-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
