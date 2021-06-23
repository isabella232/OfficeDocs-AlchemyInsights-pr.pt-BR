---
title: Habilitar autenticação SMTP e solução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077639"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="9fae6-102">Habilitar autenticação SMTP e solução de problemas</span><span class="sxs-lookup"><span data-stu-id="9fae6-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="9fae6-103">Se quiser habilitar a autenticação SMTP para uma caixa de correio ou estiver recebendo um erro "Cliente não autenticado", "Autenticação malsucedida" ou "SmtpClientAuthentication" com o código 5.7.57 ou 5.7.3 ou 5.7.139 ao tentar retransmitir emails autenticando um dispositivo ou aplicativo com o Microsoft 365, execute estas três ações para resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="9fae6-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="9fae6-104">Desabilite o [padrão de segurança do Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) alternando **Habilitar padrões de segurança** para **Não**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="9fae6-105">a.</span><span class="sxs-lookup"><span data-stu-id="9fae6-105">a.</span></span> <span data-ttu-id="9fae6-106">Entre no portal do Azure como administrador de segurança, administrador de acesso condicional ou administrador global.</span><span class="sxs-lookup"><span data-stu-id="9fae6-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="9fae6-107">b.</span><span class="sxs-lookup"><span data-stu-id="9fae6-107">b.</span></span> <span data-ttu-id="9fae6-108">Navegue até Azure Active Directory > **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="9fae6-109">c.</span><span class="sxs-lookup"><span data-stu-id="9fae6-109">c.</span></span> <span data-ttu-id="9fae6-110">Selecione **Gerenciar padrões de segurança**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="9fae6-111">d.</span><span class="sxs-lookup"><span data-stu-id="9fae6-111">d.</span></span> <span data-ttu-id="9fae6-112">Defina **Habilitar padrões de segurança** para **Não**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="9fae6-113">e.</span><span class="sxs-lookup"><span data-stu-id="9fae6-113">e.</span></span> <span data-ttu-id="9fae6-114">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-114">Select **Save**.</span></span>

2. <span data-ttu-id="9fae6-115">[Habilite o envio de cliente SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) na caixa de correio licenciada.</span><span class="sxs-lookup"><span data-stu-id="9fae6-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="9fae6-116">a.</span><span class="sxs-lookup"><span data-stu-id="9fae6-116">a.</span></span> <span data-ttu-id="9fae6-117">No Centro de administração do Microsoft 365, acesse **Usuários ativos** e selecione o usuário.</span><span class="sxs-lookup"><span data-stu-id="9fae6-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="9fae6-118">b.</span><span class="sxs-lookup"><span data-stu-id="9fae6-118">b.</span></span> <span data-ttu-id="9fae6-119">Vá para a guia Email e, em **Aplicativos de email**, selecione **Gerenciar aplicativos de email**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="9fae6-120">d.</span><span class="sxs-lookup"><span data-stu-id="9fae6-120">d.</span></span> <span data-ttu-id="9fae6-121">Verifique se o **SMTP autenticado** está marcado (habilitado).</span><span class="sxs-lookup"><span data-stu-id="9fae6-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="9fae6-122">e.</span><span class="sxs-lookup"><span data-stu-id="9fae6-122">e.</span></span> <span data-ttu-id="9fae6-123">Selecione **Salvar alterações**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="9fae6-124">[Desabilite a autenticação multifator (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na caixa de correio licenciada.</span><span class="sxs-lookup"><span data-stu-id="9fae6-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="9fae6-125">a.</span><span class="sxs-lookup"><span data-stu-id="9fae6-125">a.</span></span> <span data-ttu-id="9fae6-126">Vá para o Centro de administração do Microsoft 365 e, no menu de navegação à esquerda, selecione **Usuários** > **Usuários ativos**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="9fae6-127">b.</span><span class="sxs-lookup"><span data-stu-id="9fae6-127">b.</span></span> <span data-ttu-id="9fae6-128">Selecione **Autenticação multifator**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="9fae6-129">c.</span><span class="sxs-lookup"><span data-stu-id="9fae6-129">c.</span></span> <span data-ttu-id="9fae6-130">Selecione o usuário e desabilite a **Autenticação multifator**.</span><span class="sxs-lookup"><span data-stu-id="9fae6-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
