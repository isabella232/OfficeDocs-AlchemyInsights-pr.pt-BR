---
title: Um dos seus certificados de serviço de federação de local estiver expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274350"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um dos seus certificados de serviço de federação de local estiver expirando

Para resolver esse problema, siga estas etapas:
  
- Instale o Microsoft Azure Active Directory módulo para Windows PowerShell no computador (se o módulo já não estiver instalado). Para fazer isso, vá para o [Windows Azure Active Directory PowerShell para gráfico](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga as etapas de "cenário 1: O certificado de assinatura de token do AD FS expirado" seção de [erro "Houve um problema ao acessar o site" da AD FS quando um usuário federado entra no Office 365, Azure ou Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Siga as etapas em t[como atualizar ou reparar as configurações de um domínio federado no Office 365, Azure ou Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para obter mais informações sobre a renovação de certificados de federação, consulte [renovação de certificados para O365 e o Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

