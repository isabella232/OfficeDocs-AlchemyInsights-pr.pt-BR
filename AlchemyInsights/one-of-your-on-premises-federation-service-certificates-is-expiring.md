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
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761371"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um dos certificados do serviço de Federação no local está expirando

Para resolver esse problema, siga estas etapas:
  
- Instale o módulo Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para o [PowerShell do Azure Active Directory para o Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga as etapas na seção "cenário 1: o certificado de assinatura de token do AD FS expirado" de ["houve um problema ao acessar o site" do AD FS quando um usuário federado entra no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Siga as etapas em t[como atualizar ou reparar as configurações de um domínio federado no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para obter mais informações sobre como renovar certificados de Federação, confira [renovação de certificado para o O365 e o Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

