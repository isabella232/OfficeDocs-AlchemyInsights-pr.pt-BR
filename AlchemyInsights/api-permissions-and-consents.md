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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932085"
---
# <a name="api-permissions-and-consent"></a>Permissões e consentimento da API

Os aplicativos que se integram plataforma de identidade da Microsoft seguem um modelo de autorização que oferece aos usuários e administradores controle sobre como os dados podem ser acessados. A implementação do modelo de autorização foi atualizada plataforma de identidade da Microsoft ponto de extremidade. Ele altera como um aplicativo deve interagir com o plataforma de identidade da Microsoft. [Permissões e consentimento no ponto](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) de extremidade plataforma de identidade da Microsoft abrange os conceitos básicos desse modelo de autorização, incluindo escopos, permissões e consentimento.

A Azure Active Directory de consentimento [(Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita o desenvolvimento de aplicativos cliente nativos e web de vários locatários. Esses aplicativos permitem entrar por contas de usuário de um locatário do Azure AD diferente do que o aplicativo está registrado. Eles também podem precisar acessar APIs da Web, como a API do Microsoft Graph (para acessar o Azure AD, o Intune e os serviços no Microsoft 365) e outras APIs do serviços Microsoft, além de suas próprias APIs da Web.

