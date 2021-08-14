---
title: Problemas de consentimento do administrador
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952561"
---
# <a name="admin-consent-issues"></a>Problemas de consentimento do administrador

1. Habilita [o fluxo de trabalho de consentimento](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) do administrador para permitir que os usuários solicitem aprovação do administrador diretamente da tela de consentimento.

1. Se você ou os usuários do aplicativo estão vendo erros inesperados durante o processo de consentimento, consulte este artigo para solucionar problemas etapas: Erro inesperado ao executar o consentimento [para um aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Saiba mais sobre [o consentimento do](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)administrador no plataforma de identidade da Microsoft , como o [prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) de consentimento funciona e como avaliar uma solicitação de consentimento de administrador em todo o [locatário.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Os aplicativos que se integram plataforma de identidade da Microsoft seguem um modelo de autorização que oferece aos usuários e administradores controle sobre como os dados podem ser acessados. A implementação do modelo de autorização foi atualizada plataforma de identidade da Microsoft ponto de extremidade e altera como um aplicativo deve interagir com o plataforma de identidade da Microsoft. Consulte [Permissões e consentimento](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) no ponto de extremidade plataforma de identidade da Microsoft para uma visão geral deste modelo de autorização, incluindo escopos, permissões e consentimento.