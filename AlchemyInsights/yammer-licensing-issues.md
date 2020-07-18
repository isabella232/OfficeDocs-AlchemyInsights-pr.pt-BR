---
title: Problemas de licenciamento do Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146743"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="7ace7-102">Problemas de licenciamento do Yammer</span><span class="sxs-lookup"><span data-stu-id="7ace7-102">Yammer licensing issues</span></span>

<span data-ttu-id="7ace7-103">Todos os usuários devem ter uma licença para usar o serviço do Yammer Enterprise, mas, por padrão, o Yammer não requer que os usuários tenham uma licença para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="7ace7-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="7ace7-104">Quando um administrador muda as configurações para bloquear usuários do Microsoft 365 sem as licenças do Yammer, usuários que não tem uma licença Yammer Enterprise não podem acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="7ace7-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="7ace7-105">Para saber mais, confira [Gerenciar licenças de usuário do Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="7ace7-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="7ace7-106">Quando as licenças são removidas dos usuários, o bloco do Yammer não é mais exibido, e outros serviços podem usar a remoção da licença para ocultar recursos.</span><span class="sxs-lookup"><span data-stu-id="7ace7-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="7ace7-107">Em outros casos, os recursos ainda podem ser exibidos mas exigem uma licença para operar.</span><span class="sxs-lookup"><span data-stu-id="7ace7-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="7ace7-108">**A licença não está sendo atualizada para o usuário**</span><span class="sxs-lookup"><span data-stu-id="7ace7-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="7ace7-109">Ocasionalmente, o usuário é dado uma licença mas ainda não consegue acessar o Yammer.</span><span class="sxs-lookup"><span data-stu-id="7ace7-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="7ace7-110">Os atrasos têm maior probabilidade de ocorrer quando uma atribuição de licença em massa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="7ace7-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="7ace7-111">Os usuários do Yammer não podem ser atualizados na mesma ordem em que as licenças são modificadas no Azure AD porque o sistema é executado de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="7ace7-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="7ace7-112">Aguarde até 24 horas antes de abrir um caso de suporte para informar problemas de sincronização de licença.</span><span class="sxs-lookup"><span data-stu-id="7ace7-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="7ace7-113">**Atribuição de licenças em massa**</span><span class="sxs-lookup"><span data-stu-id="7ace7-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="7ace7-114">Licenças podem ser atribuídas pelo centro de administração ou script do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7ace7-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="7ace7-115">Para saber mais, confira [Atribuir licenças à usuários](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)e[Atribuir licenças para contas de usuários com Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="7ace7-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="7ace7-116">O suporte da Microsoft não fornece assistência criando scripts mas documentação de atribuição de licenças no Yammer está disponível.</span><span class="sxs-lookup"><span data-stu-id="7ace7-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="7ace7-117">Para saber mais, confira [Gerenciar licenças do Yammer usando Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="7ace7-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>