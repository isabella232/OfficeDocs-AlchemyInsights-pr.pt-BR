---
title: Ocultar pastas públicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945730"
---
# <a name="hide-public-folders"></a>Ocultar pastas públicas

**Para ocultar toda a árvore de pastas públicas**:

Use as etapas [neste](https://aka.ms/ControlPF) artigo para ocultar a árvore de pasta pública inteira de usuários seletivos ou de todos.

**Para ocultar uma pasta pública específica**:

1. Adicionar permissões para usuários que precisam acessar a pasta pública

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Remova o **Padrão** do usuário da **lista de permissões**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
