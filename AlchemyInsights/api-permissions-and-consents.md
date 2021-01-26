---
title: Permissões e consentimento da API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951857"
---
# <a name="api-permissions-and-consent"></a>Permissões e consentimento da API

Os aplicativos que se integram à Plataforma de Identidade da Microsoft seguem um modelo de autorização que oferece aos usuários e administradores controle sobre como os dados podem ser acessados. A implementação do modelo de autorização foi atualizada no ponto de extremidade da plataforma de identidade da Microsoft. Ele altera como um aplicativo deve interagir com a Plataforma de Identidade da Microsoft. [As permissões e o consentimento no](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ponto de extremidade da Plataforma de Identidade da Microsoft abrangem os conceitos básicos desse modelo de autorização, incluindo escopos, permissões e consentimento.

A estrutura de consentimento do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita o desenvolvimento de aplicativos cliente nativos e da Web de vários locatários. Esses aplicativos permitem o login por contas de usuário de um locatário do Azure AD diferente do aplicativo em que o aplicativo está registrado. Talvez eles também precisem acessar APIs da Web, como a API do Microsoft Graph (para acessar o Azure AD, o Intune e os serviços no Microsoft 365) e outras APIs dos serviços Microsoft, além de suas próprias APIs da Web.

