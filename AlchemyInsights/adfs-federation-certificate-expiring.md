---
title: Vencimento do certificado de Federação do ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499879"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="038ff-102">Vencimento do certificado de Federação do ADFS</span><span class="sxs-lookup"><span data-stu-id="038ff-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="038ff-103">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="038ff-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="038ff-104">Instale o módulo Microsoft Azure Active Directory para Windows PowerShell no computador (se o módulo ainda não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="038ff-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="038ff-105">Para fazer isso, vá para [gerenciar o Azure ad usando o Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="038ff-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="038ff-106">Siga as etapas na seção "cenário 1: o certificado de assinatura de token do AD FS expirado" de ["houve um problema ao acessar o site" do AD FS quando um usuário federado entra no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="038ff-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="038ff-107">Siga as etapas em [como atualizar ou reparar as configurações de um domínio federado no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="038ff-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="038ff-108">Para saber mais sobre como renovar certificados de Federação, consulte renovar [certificados de Federação para o Office 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="038ff-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
