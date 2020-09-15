---
title: Expiração do Certificado de Federação ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686702"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiração do Certificado de Federação ADFS

Para resolver esse problema, siga estas etapas:
  
1. Instale o módulo Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para [gerenciar o Azure ad usando o Windows PowerShell](https://aka.ms/aadposh).

2. Siga as etapas na seção "cenário 1: o certificado de assinatura de token do AD FS expirado" de ["houve um problema ao acessar o site" do AD FS quando um usuário federado entra no Microsoft 365, no Azure ou no Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga as etapas em [atualizar ou reparar as configurações de um domínio federado no Microsoft, no Azure ou no Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre como renovar certificados de Federação, consulte [renovar certificados de Federação para o Microsoft 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
