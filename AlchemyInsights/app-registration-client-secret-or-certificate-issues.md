---
title: Segredo do cliente de registro de aplicativo ou problemas de certificado
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951481"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Segredo do cliente de registro de aplicativo ou problemas de certificado

O segredo do cliente de aplicativo expirando?

Independentemente de como o aplicativo registrado foi criado, seja por meio do processo de registro padrão no portal de Registro de Aplicativos ou se a Entidade de Serviço foi criada em seu locatário usando o consentimento do aplicativo, um novo Segredo do Cliente precisará ser criado antes da expiração do atual e atualizado no código do aplicativo relacionado. O período máximo de validade é 2 anos. Como lembrete, o valor secreto deve ser gravado, pois ele não ficará mais visível depois de sair da página Registros do aplicativo no portal. Para obter mais informações, consulte [Início rápido: Registrar](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) um aplicativo no plataforma de identidade da Microsoft [e Práticas recomendadas para](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)o plataforma de identidade da Microsoft .

Para saber mais, consulte [Create an Azure AD app & service principal in the portal - plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
