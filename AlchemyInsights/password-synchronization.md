---
title: Sincronização de senha
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449042"
---
# <a name="password-synchronization"></a><span data-ttu-id="e380c-102">Sincronização de senha</span><span class="sxs-lookup"><span data-stu-id="e380c-102">Password synchronization</span></span>

<span data-ttu-id="e380c-103">**A Sincronização de Hash de Senha não funciona em nada**</span><span class="sxs-lookup"><span data-stu-id="e380c-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="e380c-104">Alguns problemas comuns que os clientes encontram quando a Sincronização de Hash de Senha não funciona são:</span><span class="sxs-lookup"><span data-stu-id="e380c-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="e380c-105">A conta do Active Directory usada pelo Azure AD Connect para  se comunicar  com o Active Directory local não é concedida Replicar Alterações de Diretório e Replicar Alterações de Diretório Todas as permissões, que são necessárias para sincronização de senhas - Você precisa corrigir isso concedendo essas permissões à conta do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e380c-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="e380c-106">A sincronização de hash de senha é desabilitada  depois que um administrador alterou o método User Sign-In de Sincronização de Senha para outra opção, como Federação com **AD FS** no assistente do Azure AD Connect - Você pode corrigir isso rehabilitando o recurso de sincronização **de hash** de senha no assistente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e380c-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="e380c-107">Problema de conectividade com o Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="e380c-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="e380c-108">Por exemplo, alguns controladores de domínio não são acessíveis [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) pelo Azure AD Connect ou as portas necessárias são bloqueadas pelo Firewall - Você precisa corrigir isso garantindo que a conectividade entre o servidor do Azure AD Connect e o Active Directory local funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="e380c-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="e380c-109">O servidor do Azure AD Connect está no modo de preparo, o que fará com que o servidor não consiga os hashes de senha - Para solucionar o problema, siga as etapas descritas na seção Solucionar problemas de sincronização de senha com a sincronização do [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nenhuma senha é sincronizada .</span><span class="sxs-lookup"><span data-stu-id="e380c-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="e380c-110">**A Sincronização de Hash de Senha não funciona para alguns dos meus usuários**</span><span class="sxs-lookup"><span data-stu-id="e380c-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="e380c-111">Se você reparou que o hash de senha  não está sincronizando para um usuário, use a tarefa de solução de problemas no Azure AD Connect para investigar e resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="e380c-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="e380c-112">Execute as seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="e380c-112">Perform the following tasks:</span></span>

    <span data-ttu-id="e380c-113">a.</span><span class="sxs-lookup"><span data-stu-id="e380c-113">a.</span></span> [<span data-ttu-id="e380c-114">Executar a tarefa de solução de problemas no assistente</span><span class="sxs-lookup"><span data-stu-id="e380c-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="e380c-115">b.</span><span class="sxs-lookup"><span data-stu-id="e380c-115">b.</span></span> [<span data-ttu-id="e380c-116">Use o cmdlet de solução de problemas para investigar o problema de sincronização de hash de senha para um uso específico</span><span class="sxs-lookup"><span data-stu-id="e380c-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="e380c-117">O objeto Usuário do Active Directory local está habilitado para que o Usuário altere a **senha na próxima opção de logon.**</span><span class="sxs-lookup"><span data-stu-id="e380c-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="e380c-118">Quando essa opção estiver habilitada, o usuário receberá uma senha temporária e será solicitado a alterar a senha no próximo logon.</span><span class="sxs-lookup"><span data-stu-id="e380c-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="e380c-119">O Azure AD Connect não sincroniza senhas temporárias com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e380c-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="e380c-120">Para resolver o problema acima, execute uma das seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="e380c-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="e380c-121">Peça ao usuário para entrar no aplicativo local (por exemplo, Windows Desktop) e alterar a senha.</span><span class="sxs-lookup"><span data-stu-id="e380c-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="e380c-122">A nova senha será sincronizada com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e380c-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="e380c-123">Fazer com que um administrador atualize a senha do usuário sem habilbilcar a opção O usuário deve alterar a senha no próximo **logon** e compartilhar a nova senha com o usuário.</span><span class="sxs-lookup"><span data-stu-id="e380c-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="e380c-124">O objeto Usuário do Active Directory local não **está configurado corretamente** para sincronização de objetos ou sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="e380c-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="e380c-125">Para solucionar esse problema, siga as etapas descritas na sincronização de hash de senha de solução de problemas com a sincronização [do Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="e380c-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







