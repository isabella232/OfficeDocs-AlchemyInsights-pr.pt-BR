---
title: Configurar LDAP
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
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876531"
---
# <a name="configure-ldap"></a><span data-ttu-id="e6588-102">Configurar LDAP</span><span class="sxs-lookup"><span data-stu-id="e6588-102">Configure LDAP</span></span>

<span data-ttu-id="e6588-103">Para configurar o LDAP, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="e6588-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="e6588-104">Verifique a saúde do seu domínio no [portal do Azure.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="e6588-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="e6588-105">Verifique se uma assinatura válida do Azure AD está disponível e se os Serviços de Domínio do Azure AD foram habilitados.</span><span class="sxs-lookup"><span data-stu-id="e6588-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="e6588-106">O certificado necessário para habilitar o LDAP seguro deve ser obtido de uma autoridade de certificação pública confiável ou ser um certificado auto-assinado.</span><span class="sxs-lookup"><span data-stu-id="e6588-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="e6588-107">Certifique-se de que o certificado siga as [diretrizes necessárias.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="e6588-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="e6588-108">**Certificado inválido**</span><span class="sxs-lookup"><span data-stu-id="e6588-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="e6588-109">Para renovar um certificado, siga as etapas para criar um novo certificado e recarregar: [Configurar LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="e6588-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="e6588-110">Para resolver um problema conhecido com alertas LDAP seguros nos Serviços de Domínio do Azure Active Directory, confira [Resolver alertas LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="e6588-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
