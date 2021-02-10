---
title: Sincronização de hash de senha para serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162907"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="52e68-102">Sincronização de hash de senha para serviço de domínio</span><span class="sxs-lookup"><span data-stu-id="52e68-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="52e68-103">**Se sua instância do Azure AD DS estiver solicitando que você habilite a sincronização de hash de senha**</span><span class="sxs-lookup"><span data-stu-id="52e68-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="52e68-104">Você encontra um cenário no qual está executando um ambiente híbrido com usuários sincronizando a partir de um ambiente local dos Serviços de Domínio Active Directory (AD DS) do Azure.</span><span class="sxs-lookup"><span data-stu-id="52e68-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="52e68-105">Este cenário é encontrado apesar de você ter sincronização de hash de senha do AD DS local para seu locatário do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52e68-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="52e68-106">**Causa**</span><span class="sxs-lookup"><span data-stu-id="52e68-106">**Cause**</span></span>

<span data-ttu-id="52e68-107">Isso está acontecendo porque o Azure AD Connect, por padrão, não sincroniza o New Technology LAN Manager (NTLM) herdado e os hashes de senha Kerberos necessários para o Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="52e68-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="52e68-108">**Solução alternativa**</span><span class="sxs-lookup"><span data-stu-id="52e68-108">**Workaround**</span></span> 

<span data-ttu-id="52e68-109">Você precisaria configurar o Azure AD Connect para sincronizar os hashes de senha necessários para a autenticação NTLM e Kerberos.</span><span class="sxs-lookup"><span data-stu-id="52e68-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="52e68-110">Depois que o Azure AD Connect é configurado, uma criação de conta local ou evento de alteração de senha também sincroniza os hashes de senha herdados com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="52e68-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="52e68-111">Consulte [aqui ](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) para obter mais informações sobre isso e para obter orientação sobre como habilitar a sincronização de senha em ambientes híbridos do Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="52e68-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>