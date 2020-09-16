---
title: Problemas utilizando o console de administração do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728275"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="5536b-102">Problemas utilizando o console de administração do Intune</span><span class="sxs-lookup"><span data-stu-id="5536b-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="5536b-103">**"Acesso negado" ao navegar pelo portal de administração do Intune.**</span><span class="sxs-lookup"><span data-stu-id="5536b-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="5536b-104">Se você for um membro de uma função personalizada do Intune, certifique-se de que uma licença do Intune ou Enterprise Mobility Suite (EMS) está atribuída à sua conta.</span><span class="sxs-lookup"><span data-stu-id="5536b-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="5536b-105">Se você estiver usando o Gerenciador de Configurações para gerenciar os dispositivos, certifique-se de que não faça parte da coleção de usuários do Intune para o Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="5536b-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="5536b-106">Verifique se você recebeu as permissões apropriadas do controle de administração baseado em função (RBAC) na lâmina funções do Intune.</span><span class="sxs-lookup"><span data-stu-id="5536b-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="5536b-107">Verifique se o grupo usado não é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="5536b-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="5536b-108">O Intune no portal do Azure é compatível apenas com as contas de usuário que pertencem aos grupos de segurança do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5536b-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="5536b-109">Examine seus grupos no portal do Azure > **Intune** > **Grupos**ou no portal do Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="5536b-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="5536b-110">**O usuário tem muitas permissões para a função atribuída do Intune**</span><span class="sxs-lookup"><span data-stu-id="5536b-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="5536b-111">Peça para o usuário acessar **Intune** > **funções do Intune** > **Minhas permissões** > **Exportar**para revisar as permissões concedidas.</span><span class="sxs-lookup"><span data-stu-id="5536b-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="5536b-112">**Adicionei um grupo de escopo a uma função, mas os usuários desse papel ainda poderão ver outros usuários ou dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="5536b-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="5536b-113">Os grupos de escopo não filtram usuários ou dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5536b-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="5536b-114">Grupos de escopo:</span><span class="sxs-lookup"><span data-stu-id="5536b-114">Scope groups:</span></span>

- <span data-ttu-id="5536b-115">Limitar a quem os usuários podem atribuir políticas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="5536b-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="5536b-116">Permita que somente usuários específicos executem tarefas remotas em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5536b-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="5536b-117">Para obter mais informações sobre os grupos de escopo, confira [Controle de acesso baseado em função (RBAC) com o](https://docs.microsoft.com/intune/role-based-access-control)do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5536b-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="5536b-118">**Adicionei um usuário a uma função do Intune, mas ainda temos acesso total ao console de administração do Intune.**</span><span class="sxs-lookup"><span data-stu-id="5536b-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="5536b-119">Navegue até o Intune > **Usuários** no portal do Azure e verifique se o usuário não está atribuído a nenhuma das funções a seguir no portal do Azure:</span><span class="sxs-lookup"><span data-stu-id="5536b-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="5536b-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5536b-120">Global administrator</span></span>
- <span data-ttu-id="5536b-121">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="5536b-121">Intune service administrator</span></span>
- <span data-ttu-id="5536b-122">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="5536b-122">SharePoint administrator</span></span>

<span data-ttu-id="5536b-123">Confira [Controle de acesso baseado em função (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="5536b-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="5536b-124">**Problemas de Acesso**</span><span class="sxs-lookup"><span data-stu-id="5536b-124">**Access Issues**</span></span>

<span data-ttu-id="5536b-125">Para saber mais, confira [Não é possível entrar no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="5536b-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>