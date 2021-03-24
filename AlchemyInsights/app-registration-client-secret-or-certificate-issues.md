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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123033"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Segredo do cliente de registro de aplicativo ou problemas de certificado

O segredo do cliente de aplicativo expirando?

Independentemente de como o aplicativo registrado foi criado, seja por meio do processo de registro padrão no portal de Registro de Aplicativos ou se a Entidade de Serviço foi criada em seu locatário usando o consentimento do aplicativo, um novo Segredo do Cliente precisará ser criado antes da expiração do atual e atualizado no código do aplicativo relacionado. O período máximo de validade é 2 anos. Como lembrete, o valor secreto deve ser gravado, pois ele não ficará mais visível depois de sair da página Registros do aplicativo no portal. Para obter mais informações, consulte [Início rápido: Registrar](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) um aplicativo na plataforma de identidade da Microsoft e [práticas recomendadas para a plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Para saber mais, consulte [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
