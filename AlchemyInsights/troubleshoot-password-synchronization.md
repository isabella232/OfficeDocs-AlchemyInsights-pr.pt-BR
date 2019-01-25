---
title: Solucionar problemas de sincronização de senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457080"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6228c-102">Solucionar problemas de sincronização de senha</span><span class="sxs-lookup"><span data-stu-id="6228c-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6228c-103">Para solucionar problemas em que nenhum senhas são sincronizados com a versão do Windows Azure Connect da AD 1.1.614.0 ou posterior:</span><span class="sxs-lookup"><span data-stu-id="6228c-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="6228c-104">Abra uma nova sessão do Windows PowerShell no seu servidor do Azure Connect do AD com a opção **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="6228c-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="6228c-105">Execute **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy irrestrito**.</span><span class="sxs-lookup"><span data-stu-id="6228c-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="6228c-106">Inicie o Assistente de conectar do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6228c-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="6228c-107">Navegue até o \* \* tarefas adicionais \* \* página, selecione \* \* Troubleshoot \* \* e clique em **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="6228c-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="6228c-108">Na página de solução de problemas, clique em menu **Iniciar para iniciar a solução de problemas** no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6228c-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="6228c-109">No menu principal, selecione **Solucionar problemas de sincronização de senha**.</span><span class="sxs-lookup"><span data-stu-id="6228c-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="6228c-110">No menu sub, selecione a **sincronização de senha não funciona em todos os**.</span><span class="sxs-lookup"><span data-stu-id="6228c-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="6228c-111">**Compreender os resultados da tarefa a solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6228c-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="6228c-112">A tarefa de solução de problemas executa as seguintes verificações:</span><span class="sxs-lookup"><span data-stu-id="6228c-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="6228c-113">Valida que o recurso de sincronização de senha está habilitado para seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6228c-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="6228c-114">Valida que o servidor Connect do Azure AD não está no modo de preparo.</span><span class="sxs-lookup"><span data-stu-id="6228c-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="6228c-115">Para cada conector de Active Directory local existente, (que corresponde a uma floresta existente do Active Directory):</span><span class="sxs-lookup"><span data-stu-id="6228c-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="6228c-116">Valida se o recurso de sincronização de senha está habilitado.</span><span class="sxs-lookup"><span data-stu-id="6228c-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="6228c-117">Procura eventos de pulsação de sincronização de senha nos logs de eventos do Windows.</span><span class="sxs-lookup"><span data-stu-id="6228c-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="6228c-118">Para cada domínio do Active Directory sob o conector do Active Directory local:</span><span class="sxs-lookup"><span data-stu-id="6228c-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="6228c-119">Valida que o domínio é acessível a partir do servidor Connect do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6228c-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="6228c-120">Valida que as contas de serviços de domínio Active Directory (AD DS) usadas pelo conector do Active Directory local tem o nome de usuário correto, senha e permissões necessárias para a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="6228c-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="6228c-121">Para obter mais ajuda para solucionar problemas de sincronização de senha, consulte [Troubleshoot a sincronização de senha com a sincronização do Azure Connect do AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6228c-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

