---
title: Sobre identidades no Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146742"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="61f70-102">Sobre identidades no Yammer</span><span class="sxs-lookup"><span data-stu-id="61f70-102">About identity in Yammer</span></span>

<span data-ttu-id="61f70-103">É recomendável que todas as redes sigam as seguintes etapas para evitar problemas relacionados à identidade:</span><span class="sxs-lookup"><span data-stu-id="61f70-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="61f70-104">Impor identidade do Office 365 após provisionar contas da Microsoft 365 para usuários no Azure AD para garantir que todos os usuários entrem usando suas contas principais do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="61f70-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="61f70-105">Para mais informações, confira [Impor identidade do Office 365 para usuários do Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="61f70-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="61f70-106">Consolidar várias redes do Yammer.</span><span class="sxs-lookup"><span data-stu-id="61f70-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="61f70-107">As configurações herdadas do Yammer permitem que várias redes do Yammer sejam conectadas a um locatário.</span><span class="sxs-lookup"><span data-stu-id="61f70-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="61f70-108">Para saber mais, confira [Migração de rede - Consolidar várias redes do Yammer ](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="61f70-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="61f70-109">Opcionalmente, impor licenciamento do Yammer a bloquear usuários se eles não tiverem uma licença.</span><span class="sxs-lookup"><span data-stu-id="61f70-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="61f70-110">Para saber mais, confira [Gerenciar licenças de usuário do Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="61f70-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="61f70-111">Por fim, auditar a lista de usuários das redes antigas no Yammer e suspender usuários herdados.</span><span class="sxs-lookup"><span data-stu-id="61f70-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="61f70-112">É recomendável suspender (desativar) usuários ao invés de excluí-los pois a exclusão é irreversível.</span><span class="sxs-lookup"><span data-stu-id="61f70-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="61f70-113">Para saber mais, confira [Auditar usuários do Yammer em redes conectadas ao Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Remover usuários](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="61f70-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="61f70-114">Ao configurar o Yammer seguindo essas etapas, você também poderá configurar sua rede no modo Nativo para Microsoft 365 no Yammer.</span><span class="sxs-lookup"><span data-stu-id="61f70-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="61f70-115">Para saber mais, confira[Configurar sua rede no modo Nativo para Microsoft 365 no Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="61f70-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>