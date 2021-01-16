---
title: Sincronização do serviço de domínio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876512"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="b4ea5-102">Sincronização do serviço de domínio</span><span class="sxs-lookup"><span data-stu-id="b4ea5-102">Domain service synchronization</span></span>

<span data-ttu-id="b4ea5-103">Objetos e credenciais em um domínio gerenciado dos Serviços de Domínio do Azure Active Directory (Azure AD DS) podem ser criados localmente no domínio ou sincronizados de um locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b4ea5-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="b4ea5-104">Quando você implanta pela primeira vez o Azure AD DS, uma sincronização automática de uma via é configurada e iniciada para replicar os objetos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4ea5-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="b4ea5-105">Essa sincronização de uma via continua sendo executado em segundo plano para manter o domínio gerenciado do Azure AD DS atualizado com quaisquer alterações do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4ea5-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="b4ea5-106">Nenhuma sincronização ocorre do Azure AD DS para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4ea5-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="b4ea5-107">Para obter mais detalhes sobre a sincronização do serviço de domínio do Azure Active Directory, consulte [Sincronização de Serviço de Domínio.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)</span><span class="sxs-lookup"><span data-stu-id="b4ea5-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
