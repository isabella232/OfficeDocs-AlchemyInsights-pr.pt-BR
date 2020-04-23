---
title: Um dos certificados do serviço de Federação no local está expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785291"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="a2e9a-102">Um dos certificados do serviço de Federação no local está expirando</span><span class="sxs-lookup"><span data-stu-id="a2e9a-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="a2e9a-103">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="a2e9a-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="a2e9a-104">Instale o módulo Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="a2e9a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a2e9a-105">Para fazer isso, vá para o [PowerShell do Azure Active Directory para o Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="a2e9a-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="a2e9a-106">Siga as etapas na seção "cenário 1: o certificado de assinatura de token do AD FS expirado" de ["houve um problema ao acessar o site" do AD FS quando um usuário federado entra no Microsoft 365, no Azure ou no Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a2e9a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="a2e9a-107">Siga as etapas em [como atualizar ou reparar as configurações de um domínio federado no Microsoft 365, no Azure ou no Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="a2e9a-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="a2e9a-108">Para obter mais informações sobre como renovar certificados de Federação, confira [renovação de certificado para o O365 e o Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a2e9a-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

