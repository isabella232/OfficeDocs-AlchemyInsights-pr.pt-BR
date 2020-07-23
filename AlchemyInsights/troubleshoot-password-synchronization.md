---
title: Solucionar problemas de sincronização de senha
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387865"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6bb31-102">Solucionar problemas de sincronização de senha</span><span class="sxs-lookup"><span data-stu-id="6bb31-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6bb31-103">Para solucionar problemas de sincronização de senha, comece usando esta tarefa de solução de problemas do AAD Connect para determinar por que as senhas não estão sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="6bb31-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="6bb31-104">Para começar, vá para [gerenciar a sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="6bb31-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="6bb31-105">Abra uma nova sessão do Windows PowerShell em seu servidor do Azure AD Connect e selecione a opção **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="6bb31-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6bb31-106">Execute Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="6bb31-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="6bb31-107">Inicie o assistente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6bb31-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6bb31-108">Vá até a página tarefas adicionais > **solucionar problemas**  >  **em seguida**.</span><span class="sxs-lookup"><span data-stu-id="6bb31-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="6bb31-109">Selecione **Iniciar** para abrir o menu de solução de problemas do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6bb31-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="6bb31-110">Selecione **solucionar problemas de sincronização de senha**.</span><span class="sxs-lookup"><span data-stu-id="6bb31-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="6bb31-111">Normalmente, o problema é que uma senha não é sincronizada para uma conta de usuário específica.</span><span class="sxs-lookup"><span data-stu-id="6bb31-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="6bb31-112">**Anotações** A sincronização de senha falha se a última sincronização de senha bem-sucedida ocorreu algum tempo atrás.</span><span class="sxs-lookup"><span data-stu-id="6bb31-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="6bb31-113">Para obter mais ajuda para a solução de problemas de sincronização de senha, consulte [Troubleshoot password hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6bb31-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>