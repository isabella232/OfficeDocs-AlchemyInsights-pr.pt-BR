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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952957"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiração do Certificado de Federação ADFS

Para resolver esse problema, siga estas etapas:
  
1. Instale o Microsoft Azure Active Directory módulo para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para [Gerenciar o Azure AD usando Windows PowerShell](https://aka.ms/aadposh).

2. Siga as etapas na seção "Cenário 1: o certificado de assinatura de token do AD FS expirou" da seção "Houve um problema ao acessar o site" do AD FS quando um usuário federado entra no [Microsoft 365, no Azure ou no Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga as etapas em Atualizar ou reparar as configurações de um domínio federado na [Microsoft, no Azure ou no Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre a renovação de certificados de Federação, consulte [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
