---
title: Nenhum resultado retornado durante a pesquisa/exportação de conteúdo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727211"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nenhum resultado retornado durante a pesquisa/exportação de conteúdo

Se você estiver tendo problemas com os seguintes cenários de descoberta eletrônica:

- A pesquisa/exportação de conteúdo não retorna dados ou dados inesperados
- falha de pesquisa ou exportação de descoberta eletrônica

Isso pode ser devido a determinados filtros de segurança de conformidade que foram configurados por um administrador específico e não foram comunicados a todos os administradores.

Para resolver isso, verifique se há algum filtro de segurança de conformidade que possa estar causando estes problemas:

1. Conectar-se ao PowerShell do centro de conformidade e segurança
2. Execute o seguinte comandos:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obter informações adicionais sobre filtros de segurança de conformidade, confira [permissões de filtragem para pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
