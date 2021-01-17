---
title: Atribuindo grupos à função do Microsoft Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875330"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="86528-102">Atribuindo grupos à função do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="86528-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="86528-103">Para atribuir um grupo do Microsoft Azure AD com a origem da autoridade no Microsoft Azure AD a uma função do Microsoft Azure AD, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="86528-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="86528-104">Crie um novo grupo - Para criar um novo grupo:</span><span class="sxs-lookup"><span data-stu-id="86528-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="86528-105">a.</span><span class="sxs-lookup"><span data-stu-id="86528-105">a.</span></span> <span data-ttu-id="86528-106">Entre no centro de administração do Microsoft Azure AD com permissões de **administrador de função privilegiada** ou **administrador global**.</span><span class="sxs-lookup"><span data-stu-id="86528-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="86528-107">b.</span><span class="sxs-lookup"><span data-stu-id="86528-107">b.</span></span> <span data-ttu-id="86528-108">Selecione **Azure Active Directory > Grupos > Todos os grupos > Novo grupo**.</span><span class="sxs-lookup"><span data-stu-id="86528-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="86528-109">c.</span><span class="sxs-lookup"><span data-stu-id="86528-109">c.</span></span> <span data-ttu-id="86528-110">Crie o grupo.</span><span class="sxs-lookup"><span data-stu-id="86528-110">Create the group.</span></span>

2. <span data-ttu-id="86528-111">Atribua a função ao grupo durante a criação do grupo ou após a criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="86528-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="86528-112">a.</span><span class="sxs-lookup"><span data-stu-id="86528-112">a.</span></span> <span data-ttu-id="86528-113">Para atribuir uma função ao grupo no momento da sua criação, altere as **funções do Microsoft Azure AD que podem ser atribuídas ao grupo** e crie o grupo.</span><span class="sxs-lookup"><span data-stu-id="86528-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="86528-114">b.</span><span class="sxs-lookup"><span data-stu-id="86528-114">b.</span></span> <span data-ttu-id="86528-115">Para atribuir uma função ao grupo após sua criação, navegue até a guia **Funções atribuídas** para o grupo recém-criado e atribua a função ao grupo.</span><span class="sxs-lookup"><span data-stu-id="86528-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="86528-116">**Gerenciar a associação de um grupo atribuído à função do Microsoft Azure AD**</span><span class="sxs-lookup"><span data-stu-id="86528-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="86528-117">Para evitar a elevação de privilégios, por padrão, apenas administradores com funções privilegiadas e administradores globais podem modificar a associação de um grupo que é atribuído a uma função.</span><span class="sxs-lookup"><span data-stu-id="86528-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="86528-118">No entanto, eles podem escolher atribuir um proprietário a esse grupo e delegar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="86528-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="86528-119">Para obter mais detalhes sobre como atribuir grupos de nuvem a funções do Microsoft Azure AD, confira [Atribuir funções do AD ao grupo de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="86528-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="86528-120">Para obter mais detalhes sobre a solução de problemas de funções atribuídas a grupos de nuvem, confira [Solucionar problemas de funções atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="86528-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





