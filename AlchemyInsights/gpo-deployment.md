---
title: Implantação de GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067828"
---
# <a name="gpo-deployment"></a>Implantação de GPO

As configurações de objetos de usuário e de computador no Azure AD DS (Azure Active Directory Domain Services) são frequentemente gerenciadas usando GPOs (Objetos de Política de Grupo). O Azure AD DS inclui GPOs internos para contêineres de Usuários do AADDC e de Computadores do AADDC. Personalize os GPOs internos para configurar a política de grupo conforme necessário para seu ambiente. Os membros do grupo de administradores do Azure AD DC têm privilégios de administração de políticas de grupo no domínio do Azure AD DS, e também podem criar UOs (unidades organizacionais) e GPOs personalizados. Para obter mais informações sobre o que é a política de grupo e como ela funciona, consulte [Visão geral da Política de Grupo.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Em um ambiente híbrido, as políticas de grupo configuradas em um ambiente AD DS local não são sincronizadas com o Azure AD DS. Para definir as configurações de usuários ou computadores no Azure AD DS, edite um dos GPOs padrão ou crie um GPO personalizado.

Este artigo [Gerenciar Política de Grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) mostra como instalar as ferramentas do Gerenciamento de Política de Grupo, como editar os GPOs internos e como criar GPOs personalizados.
