---
title: Problema ao ingressar em VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884551"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="b0d36-102">Problema ao ingressar em VMs</span><span class="sxs-lookup"><span data-stu-id="b0d36-102">Issue joining VMs</span></span>

<span data-ttu-id="b0d36-103">Para resolver problemas que ocorrem ao tentar ingressar em VMs, execute as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="b0d36-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="b0d36-104">Tente entrar usando o formato **UPN** (por exemplo, 'joeuser@contoso.com') em vez do formato **SAMAccountName** ('CONTOSO\joeuser').</span><span class="sxs-lookup"><span data-stu-id="b0d36-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="b0d36-105">Certifique-se de ter habilitado a sincronização de senha de acordo com as etapas descritas no guia de *Introdução*.</span><span class="sxs-lookup"><span data-stu-id="b0d36-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="b0d36-106">Certifique-se de que a conta de usuário afetada não seja uma conta externa no locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b0d36-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="b0d36-107">Os usuários externos não podem entrar no domínio gerenciado, pois os Azure AD Domain Services não têm credenciais para essas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="b0d36-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="b0d36-108">Se a conta de usuário afetada for uma conta de usuário somente na nuvem, verifique se os usuários alteraram suas senhas depois de habilitar os Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="b0d36-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="b0d36-109">Essa etapa faz com que os hashes de credencial obrigatório para os Azure AD Domain Services sejam gerados.</span><span class="sxs-lookup"><span data-stu-id="b0d36-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="b0d36-110">Se as contas de usuário afetadas forem sincronizadas de um diretório local, verifique se a versão recomendada do Azure AD Connect foi configurada para executar uma sincronização completa.</span><span class="sxs-lookup"><span data-stu-id="b0d36-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="b0d36-111">Se o problema persistir após a confirmação da Etapa 4, execute os seguintes comandos em seu computador de sincronização:</span><span class="sxs-lookup"><span data-stu-id="b0d36-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="b0d36-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="b0d36-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>