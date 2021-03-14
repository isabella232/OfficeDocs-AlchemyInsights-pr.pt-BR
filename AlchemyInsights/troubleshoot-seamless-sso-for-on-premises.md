---
title: Solucionar problemas de SSO (Logon Único) Contínuo local
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753379"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="cd564-102">Solucionar problemas de SSO (Logon Único) Contínuo local</span><span class="sxs-lookup"><span data-stu-id="cd564-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="cd564-103">Para resolver problemas de SSO (Logon Único) Contínuo, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="cd564-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="cd564-104">**Como posso sobrepor a chave de descriptografia Kerberos da conta do computador AZUREADSSO?** </span><span class="sxs-lookup"><span data-stu-id="cd564-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="cd564-105">É altamente recomendável que você sobreponha a chave de descriptografia Kerberos pelo menos a cada 30 dias.</span><span class="sxs-lookup"><span data-stu-id="cd564-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="cd564-106">Para fazer isso manualmente, confira [Como sobrepor chaves de descriptografia Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="cd564-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="cd564-107">**Configurar o SSO Contínuo**</span><span class="sxs-lookup"><span data-stu-id="cd564-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="cd564-108">Para implantar o SSO Contínuo, siga as etapas em[Logo Único Contínuo do Azure Active Directory: Início Rápido](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="cd564-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="cd564-109">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="cd564-109">**Advisory**</span></span>

- <span data-ttu-id="cd564-110">[Logo Único Contínuo do Azure Active Directory: Perguntas frequentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) – Neste artigo, abordamos as perguntas mais frequentes sobre o Logo Único Contínuo do Azure Active Directory (SSO Contínuo).</span><span class="sxs-lookup"><span data-stu-id="cd564-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="cd564-111">Continue verificando sempre se há novo conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cd564-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="cd564-112">[P e R da Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Esse artigo fornece informações sobre como fazer solicitações de recursos ou fazer perguntas técnicas sobre o SSO Contínuo.</span><span class="sxs-lookup"><span data-stu-id="cd564-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="cd564-113">**Solucionar problemas**</span><span class="sxs-lookup"><span data-stu-id="cd564-113">**Troubleshoot**</span></span>

<span data-ttu-id="cd564-114">[Solucionar problemas de Logon Único Contínuo do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) – Esse artigo ajuda a encontrar informações sobre solução de problemas comuns em relação ao Logo Único Contínuo (SSO Contínuo) do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cd564-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







