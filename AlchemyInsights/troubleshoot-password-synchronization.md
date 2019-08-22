---
title: Solucionar problemas de sincronização de senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533795"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="af2ae-102">Solucionar problemas de sincronização de senha</span><span class="sxs-lookup"><span data-stu-id="af2ae-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="af2ae-103">Para solucionar problemas em que nenhuma senha é sincronizada com o Azure AD Connect versão 1.1.614.0 ou posterior:</span><span class="sxs-lookup"><span data-stu-id="af2ae-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="af2ae-104">Abra uma nova sessão do Windows PowerShell em seu servidor do Azure AD Connect com a opção **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="af2ae-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="af2ae-105">Execute **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="af2ae-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="af2ae-106">Inicie o assistente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="af2ae-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="af2ae-107">Navegue até a página **tarefas adicionais** , selecione **solução de problemas**e clique em **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="af2ae-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="af2ae-108">Na página solução de problemas, clique em **Iniciar para iniciar o menu solução de problemas** no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="af2ae-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="af2ae-109">No menu principal, selecione **solucionar problemas de sincronização de senha**.</span><span class="sxs-lookup"><span data-stu-id="af2ae-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="af2ae-110">No menu sub, selecione a **sincronização de senha não funciona de**forma alguma.</span><span class="sxs-lookup"><span data-stu-id="af2ae-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="af2ae-111">**Entender os resultados da tarefa de solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="af2ae-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="af2ae-112">A tarefa de solução de problemas executa as seguintes verificações:</span><span class="sxs-lookup"><span data-stu-id="af2ae-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="af2ae-113">Valida que o recurso de sincronização de senha está habilitado para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="af2ae-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="af2ae-114">Valida se o servidor do Azure AD Connect não está no modo de preparação.</span><span class="sxs-lookup"><span data-stu-id="af2ae-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="af2ae-115">Para cada conector local existente do Active Directory (que corresponde a uma floresta existente do Active Directory):</span><span class="sxs-lookup"><span data-stu-id="af2ae-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="af2ae-116">Valida se o recurso de sincronização de senha está habilitado.</span><span class="sxs-lookup"><span data-stu-id="af2ae-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="af2ae-117">Procura eventos de pulsação de sincronização de senha nos logs de eventos de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="af2ae-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="af2ae-118">Para cada domínio do Active Directory sob o conector local do Active Directory:</span><span class="sxs-lookup"><span data-stu-id="af2ae-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="af2ae-119">Valida se o domínio pode ser acessado pelo servidor do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="af2ae-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="af2ae-120">Valida que as contas dos serviços de domínio Active Directory (AD DS) usadas pelo conector do Active Directory local tem o nome de usuário, senha e permissões corretos necessários para a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="af2ae-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="af2ae-121">Para saber mais sobre como solucionar problemas de sincronização de senha, confira [solucionar problemas de sincronização de senha com o Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="af2ae-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  