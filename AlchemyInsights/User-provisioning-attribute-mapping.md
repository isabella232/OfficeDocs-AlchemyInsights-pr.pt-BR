---
title: Mapeamento de atributo de provisionamento do usuário
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935333"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="110fc-102">Mapeamento de atributo de provisionamento do usuário</span><span class="sxs-lookup"><span data-stu-id="110fc-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="110fc-103">Para solucionar problemas conhecidos de mapeamento de atributo, consulte [Mapeamentos de atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="110fc-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="110fc-104">O Microsoft Azure Active Directory (AD) oferece suporte ao provisionamento do usuário para aplicativos SaaS de terceiros, como o Salesforce, G Suite e outros.</span><span class="sxs-lookup"><span data-stu-id="110fc-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="110fc-105">Se você habilitar o provisionamento do usuário para um aplicativo SaaS de terceiros, o portal do Azure controlará seus valores de atributo por meio de mapeamentos de atributo.</span><span class="sxs-lookup"><span data-stu-id="110fc-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="110fc-106">Para saber como personalizar os mapeamentos de atributo padrão, confira [Personalizar mapeamentos de atributo de provisionamento de usuário para aplicativos SaaS no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="110fc-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="110fc-107">Para saber mais sobre o provisionamento de usuários do aplicativo SaaS, confira [O que é o provisionamento automático do usuário do aplicativo SaaS no Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning).</span><span class="sxs-lookup"><span data-stu-id="110fc-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="110fc-108">Ao personalizar mapeamentos de atributo para provisionamento do usuário, você pode descobrir que o atributo que você deseja mapear não aparece na lista de atributos de Origem.</span><span class="sxs-lookup"><span data-stu-id="110fc-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="110fc-109">O artigo [Sincronizar um atributo do seu Active Directory local para o Azure AD para provisionar um aplicativo](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) mostra como adicionar o atributo ausente sincronizando-o do seu AD local para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="110fc-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
