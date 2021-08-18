---
title: Política de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: 5bccaedda08e2c948a15c0b32c6f6eeecfc8bd4c4555b25291f294fe5deb3019
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088780"
---
# <a name="group-policy"></a>Política de grupo

As configurações de objetos de usuário e de computador no Azure AD DS (Azure Active Directory Domain Services) são frequentemente gerenciadas usando GPOs (Objetos de Política de Grupo). O Azure AD DS inclui GPOs internos para contêineres de Usuários do AADDC e de Computadores do AADDC. Personalize os GPOs internos para configurar a política de grupo conforme necessário para seu ambiente. Os membros do grupo de administradores do Azure AD DC têm privilégios de administração de políticas de grupo no domínio do Azure AD DS, e também podem criar UOs (unidades organizacionais) e GPOs personalizados. Para saber mais sobre o que é política de grupo e como ela funciona, confira [Visão geral da Política de Grupo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Em um ambiente híbrido, as políticas de grupo configuradas em um ambiente AD DS local não são sincronizadas com o Azure AD DS. Para definir as configurações de usuários ou computadores no Azure AD DS, edite um dos GPOs padrão ou crie um GPO personalizado.

Este artigo [Gerenciar Política de Grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) mostra como instalar as ferramentas do Gerenciamento de Política de Grupo, como editar os GPOs internos e como criar GPOs personalizados.



