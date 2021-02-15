---
title: Política de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243888"
---
# <a name="group-policy"></a><span data-ttu-id="0579a-102">Política de grupo</span><span class="sxs-lookup"><span data-stu-id="0579a-102">Group policy</span></span>

<span data-ttu-id="0579a-103">As configurações de objetos de usuário e de computador no Azure AD DS (Azure Active Directory Domain Services) são frequentemente gerenciadas usando GPOs (Objetos de Política de Grupo).</span><span class="sxs-lookup"><span data-stu-id="0579a-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="0579a-104">O Azure AD DS inclui GPOs internos para contêineres de Usuários do AADDC e de Computadores do AADDC.</span><span class="sxs-lookup"><span data-stu-id="0579a-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="0579a-105">Personalize os GPOs internos para configurar a política de grupo conforme necessário para seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="0579a-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="0579a-106">Os membros do grupo de administradores do Azure AD DC têm privilégios de administração de políticas de grupo no domínio do Azure AD DS, e também podem criar UOs (unidades organizacionais) e GPOs personalizados.</span><span class="sxs-lookup"><span data-stu-id="0579a-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="0579a-107">Para saber mais sobre o que é política de grupo e como ela funciona, confira [Visão geral da Política de Grupo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="0579a-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="0579a-108">Em um ambiente híbrido, as políticas de grupo configuradas em um ambiente AD DS local não são sincronizadas com o Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0579a-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="0579a-109">Para definir as configurações de usuários ou computadores no Azure AD DS, edite um dos GPOs padrão ou crie um GPO personalizado.</span><span class="sxs-lookup"><span data-stu-id="0579a-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="0579a-110">Este artigo [Gerenciar Política de Grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) mostra como instalar as ferramentas do Gerenciamento de Política de Grupo, como editar os GPOs internos e como criar GPOs personalizados.</span><span class="sxs-lookup"><span data-stu-id="0579a-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



