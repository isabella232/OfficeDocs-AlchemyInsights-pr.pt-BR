---
title: Problemas de gerenciamento de usuários
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897437"
---
# <a name="user-management-issues"></a><span data-ttu-id="2d4b3-102">Problemas de gerenciamento de usuários</span><span class="sxs-lookup"><span data-stu-id="2d4b3-102">User management issues</span></span>

<span data-ttu-id="2d4b3-103">**O que acontece com os atuais usuários atribuídos ao aplicativo se eu desabilitar a propriedade ‘Atribuição de usuário necessária’ (definir esta propriedade para Não)?**</span><span class="sxs-lookup"><span data-stu-id="2d4b3-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="2d4b3-104">Desabilitar **Atribuição de usuário necessária** NÃO afeta os usuários atribuídos atuais.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="2d4b3-105">Desabilitar esta propriedade apenas permite que todos os usuários acessem o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="2d4b3-106">Todos os usuários listados e aqueles usuários atribuídos a grupos no aplicativo ainda serão válidos.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="2d4b3-107">Para restringir seu aplicativo a um conjunto específico de usuários, consulte - [Restringir aplicativo do Azure AD a um conjunto específico de usuários - Plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="2d4b3-108">Para atribuir usuários e grupos a aplicativos empresariais no Azure Active Directory (Azure AD), seja a partir do portal do Azure ou usando o PowerShell, consulte [Gerenciar atribuição de usuário para um aplicativo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="2d4b3-109">Para delegar a criação de aplicativo e permissões de gerenciamento, consulte [Delegar permissões de administrador para gerenciamento de aplicativo - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="2d4b3-110">**Ocultar de usuários aplicativos empresariais específicos** - Siga as seguintes etapas para ocultar todos os Microsoft 365 Apps do painel **MyApps**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="2d4b3-111">Os aplicativos ainda estarão visíveis no Portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="2d4b3-112">Entre no portal do Azure como um administrador global do seu diretório.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="2d4b3-113">Selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="2d4b3-114">Selecione **Usuários**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="2d4b3-115">Selecione **Configurações de usuário**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="2d4b3-116">Em **aplicativos Enterprise**, clique em **Gerenciar como os usuários finais iniciam e exibem seus aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="2d4b3-117">Para **Usuários somente podem ver os Office 365 apps no Portal do Office 365**, clique em **Sim**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="2d4b3-118">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="2d4b3-119">Para saber mais, consulte [Ocultar um aplicativo Enterprise da experiência do usuário no Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="2d4b3-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="2d4b3-120">Se você oferecer um aplicativo de Software como Serviço (SaaS) a muitas organizações, você pode configurar seu aplicativo para aceitar entradas a partir de qualquer locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="2d4b3-121">Esta configuração é chamada "tornando seu aplicativo multilocatário".</span><span class="sxs-lookup"><span data-stu-id="2d4b3-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="2d4b3-122">Usuários em todos os locatários do Azure AD poderão entrar no seu aplicativo após consentir usar a conta deles com o esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="2d4b3-123">Para mais informações, consulte [Construir aplicativos que conectem usuários do Azure AD - Plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="2d4b3-124">**Como um usuário final pode acessar o aplicativo depois que ele(a) tenha sido atribuído(a) ao aplicativo?**</span><span class="sxs-lookup"><span data-stu-id="2d4b3-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="2d4b3-125">Cada aplicativo numa folha do aplicativo Enterprise tem um link para os usuários finais acessarem.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="2d4b3-126">Os usuários também podem acessar o portal **Myapps** de uma forma fácil.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="2d4b3-127">**Quer saber quais aplicativos e tipos de aplicativos estão sendo usados pelos usuários?**</span><span class="sxs-lookup"><span data-stu-id="2d4b3-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="2d4b3-128">Você pode baixar relatórios de entrada dos últimos 30 dias do **portal.azure.com > Azure Active directory> Entradas> baixar relatórios**.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="2d4b3-129">Aprenda como [Conceder a locatário amplo consentimento de administrador a um aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) e [Configurar como usuários finais dão consentimento a aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="2d4b3-130">Entenda [como o consentimento funciona](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) e [Gerencie consentimento a aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="2d4b3-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>

