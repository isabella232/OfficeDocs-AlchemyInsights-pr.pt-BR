---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685586"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="73f69-102">Bloqueando a autenticação herdada</span><span class="sxs-lookup"><span data-stu-id="73f69-102">Blocking legacy authentication</span></span>

<span data-ttu-id="73f69-103">A autenticação herdada é um termo que se refere a uma solicitação de autenticação feita por:</span><span class="sxs-lookup"><span data-stu-id="73f69-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="73f69-104">Clientes do Office mais antigos que não usam autenticação moderna (por exemplo, cliente do Office 2010).</span><span class="sxs-lookup"><span data-stu-id="73f69-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="73f69-105">Qualquer cliente que use protocolos de email herdados, como IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="73f69-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="73f69-106">Para obter mais informações sobre o bloqueio de autenticação herdada e a habilitação da autenticação moderna, consulte [bloqueio de autenticação herdada](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="73f69-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="73f69-107">Os padrões de segurança no Azure Active Directory (Azure AD) facilitam a segurança e a proteção da sua organização.</span><span class="sxs-lookup"><span data-stu-id="73f69-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="73f69-108">Os padrões de segurança contêm configurações de segurança pré-configuradas para ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="73f69-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="73f69-109">Para obter mais informações sobre os padrões de segurança, consulte [o que são padrões de segurança?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="73f69-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="73f69-110">**Observação**: se o seu locatário foi criado no ou após o 22Nd de outubro de 2019, é possível que você esteja enfrentando o novo comportamento seguro-por padrão e já tenha padrões de segurança habilitados no locatário.</span><span class="sxs-lookup"><span data-stu-id="73f69-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="73f69-111">Em um esforço para proteger todos os nossos usuários, os padrões de segurança são implantados em todos os novos locatários criados.</span><span class="sxs-lookup"><span data-stu-id="73f69-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
