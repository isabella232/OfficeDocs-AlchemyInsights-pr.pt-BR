---
title: Resolver problemas de certificado de assinatura SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529148"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="41026-102">Resolver problemas de certificado de Assinatura SAML</span><span class="sxs-lookup"><span data-stu-id="41026-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="41026-103">Para resolver o problema do certificado de assinatura SAML, execute as seguintes etapas recomendadas:</span><span class="sxs-lookup"><span data-stu-id="41026-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="41026-104">Quando você adiciona um aplicativo empresarial que oferece suporte ao SSO, o Azure gera um certificado que é chamado de [Certificado de assinatura SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="41026-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="41026-105">Este certificado tem uma data de validade de 3 anos.</span><span class="sxs-lookup"><span data-stu-id="41026-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="41026-106">Para alterar a data de validade do seu certificado, consulte [Personalize a data de expiração do seu certificado de federação e passe-o para um novo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="41026-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="41026-107">O Azure usará esse certificado para assinar os tokens SAML solicitados pelo aplicativo e enviá-los ao aplicativo para um SSO bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="41026-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="41026-108">Para que isso seja concluído, baixe o certificado do portal do Azure e envie-o ao fornecedor do aplicativo para concluir o processo de SSO.</span><span class="sxs-lookup"><span data-stu-id="41026-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="41026-109">Após a conclusão desse processo, seu aplicativo confiará neste certificado e todos os tokens SAML assinados por este certificado serão aceitos pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41026-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="41026-110">Se esse certificado expirar, crie um novo certificado, atualize-o para o fornecedor do aplicativo e torne-o ativo no lado do Azure.</span><span class="sxs-lookup"><span data-stu-id="41026-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="41026-111">Para mais informações, consulte[Renove um certificado que irá expirar em breve](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="41026-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="41026-112">Se o certificado expirar, o usuário não será bloqueado.</span><span class="sxs-lookup"><span data-stu-id="41026-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="41026-113">[Adicione um endereço de e-mail para notificações](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)a ser recebido antes que o certificado atual expire.</span><span class="sxs-lookup"><span data-stu-id="41026-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="41026-114">A etapa 4 é opcional.</span><span class="sxs-lookup"><span data-stu-id="41026-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="41026-115">Altere as opções de assinatura de certificado SAML de um aplicativo e o algoritmo de assinatura de certificado.</span><span class="sxs-lookup"><span data-stu-id="41026-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="41026-116">Para mais informações, consulte [Alterar opções de assinatura de certificado e algoritmo de assinatura](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="41026-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

