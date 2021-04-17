---
title: Expiração do Certificado de Federação ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821939"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiração do Certificado de Federação ADFS

Para resolver esse problema, siga estas etapas:
  
1. Instale o Módulo do Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para [Gerenciar o Azure AD usando Windows PowerShell](https://aka.ms/aadposh).

2. Siga as etapas na seção "Cenário 1: o certificado de assinatura de token do AD FS expirou" da seção "Houve um problema ao acessar o site" do AD FS quando um usuário federado entra no [Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga as etapas em Atualizar ou reparar as configurações de um domínio federado na [Microsoft, no Azure ou no Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre a renovação de certificados de Federação, consulte [Renovar certificados de federação para o Microsoft 365 e o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
