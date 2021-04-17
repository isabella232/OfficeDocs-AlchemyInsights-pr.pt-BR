---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820166"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="4a395-102">Bloqueando a autenticação herdda</span><span class="sxs-lookup"><span data-stu-id="4a395-102">Blocking legacy authentication</span></span>

<span data-ttu-id="4a395-103">A autenticação herdada é um termo que se refere a uma solicitação de autenticação feita por:</span><span class="sxs-lookup"><span data-stu-id="4a395-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="4a395-104">Clientes mais antigos do Office que não usam autenticação moderna (por exemplo, cliente do Office 2010).</span><span class="sxs-lookup"><span data-stu-id="4a395-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="4a395-105">Qualquer cliente que use protocolos de email herdados, como IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="4a395-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="4a395-106">Para obter mais informações sobre como bloquear a autenticação herdda e habilbilizar a autenticação moderna, consulte [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="4a395-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="4a395-107">Os padrões de segurança no Azure Active Directory (Azure AD) facilitam a segurança e ajudam a proteger sua organização.</span><span class="sxs-lookup"><span data-stu-id="4a395-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="4a395-108">Os padrões de segurança contêm configurações de segurança pré-configuradas para ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="4a395-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="4a395-109">Para obter mais informações sobre os padrões de segurança, consulte [O que são padrões de segurança?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="4a395-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="4a395-110">**Observação**: se seu locatário foi criado em ou após 22 de outubro de 2019, é possível que você esteja experimentando o novo comportamento seguro por padrão e já tenha os padrões de segurança habilitados em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="4a395-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="4a395-111">Em um esforço para proteger todos os nossos usuários, os padrões de segurança estão sendo lançados para todos os novos locatários criados.</span><span class="sxs-lookup"><span data-stu-id="4a395-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
