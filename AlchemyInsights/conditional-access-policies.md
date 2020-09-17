---
title: Políticas de Acesso Condicional
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 25dc98397920e4fbf28895f5961f154381e11c92
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812247"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="2ae57-102">Políticas de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="2ae57-102">Conditional Access policies</span></span>

<span data-ttu-id="2ae57-103">O Acesso Condicional é um recurso do Azure AD que permite impor controles no acesso a aplicativos em seu ambiente, todos baseados em condições específicas e gerenciados a partir de um local central.</span><span class="sxs-lookup"><span data-stu-id="2ae57-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="2ae57-104">Saiba mais sobre o [Acesso Condicional do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="2ae57-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="2ae57-105">**Observação**: caso seu locatário tenha sido criado após o dia 21 de outubro de 2019, e você estiver recebendo solicitações de MFA inesperadas, provavelmente os [padrões de segurança](https://aka.ms/securitydefaults) foram habilitados em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="2ae57-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="2ae57-106">**Para Gerenciar padrões de segurança**</span><span class="sxs-lookup"><span data-stu-id="2ae57-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="2ae57-107">Entre no [centro de administração](https://go.microsoft.com/fwlink/p/?linkid=834822) com as suas credenciais de administrador global.</span><span class="sxs-lookup"><span data-stu-id="2ae57-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="2ae57-108">Vá para [Propriedades do Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="2ae57-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="2ae57-109">Na parte inferior da página, clique em **Gerenciar padrões de segurança**.</span><span class="sxs-lookup"><span data-stu-id="2ae57-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="2ae57-110">Clique em **Sim** para habilitar os padrões de segurança ou em **Não** para desabilitá-los.</span><span class="sxs-lookup"><span data-stu-id="2ae57-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
