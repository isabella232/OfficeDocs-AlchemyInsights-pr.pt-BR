---
title: Função de gerenciamento de identidade privilegiada
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086198"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="81708-102">Função de gerenciamento de identidade privilegiada (PIM)</span><span class="sxs-lookup"><span data-stu-id="81708-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="81708-103">**As permissões não são concedidas após a ativação de uma função**</span><span class="sxs-lookup"><span data-stu-id="81708-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="81708-104">Quando você ativa uma função no Azure AD Privileged Identity Management (PIM), a ativação pode não ser propagada instantaneamente para todos os portais que exigem a função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="81708-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="81708-105">Às vezes, mesmo que a alteração seja propagada, o cache da Web em um portal pode fazer com que a alteração não tenha efeito imediato.</span><span class="sxs-lookup"><span data-stu-id="81708-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="81708-106">Se a ativação estiver atrasada, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="81708-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="81708-107">Saia do portal do Azure e entre novamente.</span><span class="sxs-lookup"><span data-stu-id="81708-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="81708-108">Ao ativar uma função do Azure AD ou uma função de recurso do Azure, você verá os estágios da ativação.</span><span class="sxs-lookup"><span data-stu-id="81708-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="81708-109">Depois que todos os estágios forem concluídos, você verá um link de "desconexão".</span><span class="sxs-lookup"><span data-stu-id="81708-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="81708-110">Você pode usar esse link para sair. Isso resolverá a maioria dos casos de atraso de ativação.</span><span class="sxs-lookup"><span data-stu-id="81708-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="81708-111">No PIM, verifique se você está listado como o membro da função.</span><span class="sxs-lookup"><span data-stu-id="81708-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="81708-112">Se você estiver ativando a função de administrador do Exchange, certifique-se de sair e entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="81708-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="81708-113">Se o problema persistir, abra um tíquete de suporte e aumente isso como um problema.</span><span class="sxs-lookup"><span data-stu-id="81708-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="81708-114">Se você estiver usando a função de administrador do Exchange para acessar o centro de segurança e conformidade, consulte a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="81708-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="81708-115">Se você estiver ativando uma função para acessar o centro de segurança e conformidade ou se estiver ativando a função de administrador do SharePoint, você terá um atraso de ativação de alguns minutos até algumas horas.</span><span class="sxs-lookup"><span data-stu-id="81708-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="81708-116">Esse é um problema conhecido e estamos trabalhando ativamente com essas equipes para resolver esse problema o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="81708-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="81708-117">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="81708-117">For more information, see:</span></span>

- [<span data-ttu-id="81708-118">Ativar minhas funções do Azure AD no PIM</span><span class="sxs-lookup"><span data-stu-id="81708-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="81708-119">Ativar minhas funções de recurso do Azure no PIM</span><span class="sxs-lookup"><span data-stu-id="81708-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="81708-120">**As permissões não são removidas após a desativação de uma função ou a ativação da função expira**</span><span class="sxs-lookup"><span data-stu-id="81708-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="81708-121">Quando você desativa uma função no Azure AD Privileged Identity Management ou quando um período de ativação de função expira, pode haver um atraso para você continuar a ter acesso.</span><span class="sxs-lookup"><span data-stu-id="81708-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="81708-122">Se a desativação estiver atrasada, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="81708-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="81708-123">Se você estiver desativando a função de administrador do Exchange ou se o período de ativação da função expirar, e você notar um atraso significativo antes de as permissões serem removidas, abra um tíquete de suporte e informe o engenheiro de suporte para ajudá-lo a arquivar uma permissão com a equipe de gerenciamento de acesso privilegiado (PAM) no Office sobre esse problema.</span><span class="sxs-lookup"><span data-stu-id="81708-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="81708-124">Se o período de ativação tiver expirado, mas você ainda tiver a sessão do navegador aberta, feche o navegador.</span><span class="sxs-lookup"><span data-stu-id="81708-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="81708-125">Você pode continuar a usar a função até fechar essa sessão.</span><span class="sxs-lookup"><span data-stu-id="81708-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="81708-126">Esse é um problema conhecido e estamos examinando uma possível correção para revogar ativamente cada sessão, uma vez que a ativação tenha expirado.</span><span class="sxs-lookup"><span data-stu-id="81708-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="81708-127">Se o seu atraso for diferente desses dois cenários, abra um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="81708-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
