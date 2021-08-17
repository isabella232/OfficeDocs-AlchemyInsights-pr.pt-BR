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
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314408"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Resolver problemas de certificado de Assinatura SAML

Para resolver o problema do certificado de assinatura SAML, execute as seguintes etapas recomendadas:

1. Quando você adiciona um aplicativo empresarial que oferece suporte ao SSO, o Azure gera um certificado que é chamado de [Certificado de assinatura SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Este certificado tem uma data de validade de 3 anos. Para alterar a data de validade do seu certificado, consulte [Personalize a data de expiração do seu certificado de federação e passe-o para um novo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. O Azure usará esse certificado para assinar os tokens SAML solicitados pelo aplicativo e enviá-los ao aplicativo para um SSO bem-sucedido. Para que isso seja concluído, baixe o certificado do portal do Azure e envie-o ao fornecedor do aplicativo para concluir o processo de SSO.

Após a conclusão desse processo, seu aplicativo confiará neste certificado e todos os tokens SAML assinados por este certificado serão aceitos pelo aplicativo.

3. Se esse certificado expirar, crie um novo certificado, atualize-o para o fornecedor do aplicativo e torne-o ativo no lado do Azure. Para mais informações, consulte[Renove um certificado que irá expirar em breve](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

**Observação**: se o certificado expirar, o usuário não será bloqueado.

4. [Adicione um endereço de e-mail para notificações](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)a ser recebido antes que o certificado atual expire.

**Observação**: a etapa 4 é opcional.

5. Altere as opções de assinatura de certificado SAML de um aplicativo e o algoritmo de assinatura de certificado. Para mais informações, consulte [Alterar opções de assinatura de certificado e algoritmo de assinatura](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

