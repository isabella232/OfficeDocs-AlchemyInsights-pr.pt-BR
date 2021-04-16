---
title: Um de seus Certificados de Serviço de Federação local está expirando
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810040"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um de seus Certificados de Serviço de Federação local está expirando

Para resolver esse problema, siga estas etapas:
  
- Instale o Módulo do Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para [o Azure Active Directory PowerShell para Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga as etapas na seção "Cenário 1: o certificado de assinatura de token do AD FS expirou" da seção "Houve um problema ao acessar o site" do AD FS quando um usuário federado entra no [Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Siga as etapas em Como atualizar ou reparar as configurações de um domínio federado no [Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para obter mais informações sobre a renovação de certificados de Federação, consulte [Renovação de certificados para o O365 e o Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

