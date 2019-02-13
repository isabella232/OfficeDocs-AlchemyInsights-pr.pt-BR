---
title: Federação do ADFS expiração de certificado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925368"
---
# <a name="adfs-federation-certificate-expiring"></a>Federação do ADFS expiração de certificado

Para resolver esse problema, siga estas etapas:
  
1. Instale o Microsoft Azure Active Directory módulo para Windows PowerShell no computador (se o módulo já não estiver instalado). Para fazer isso, vá para [Gerenciar o Azure AD usando o Windows PowerShell](https://aka.ms/aadposh).
    
2. Siga as etapas de "cenário 1: O certificado de assinatura de token do AD FS expirado" seção de [erro "Houve um problema ao acessar o site" da AD FS quando um usuário federado entra no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Siga as etapas em [como atualizar ou reparar as configurações de um domínio federado no Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Para saber mais sobre a renovação de certificados de federação, consulte [Renovar certificados de federação para Office 365 e Windows Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

