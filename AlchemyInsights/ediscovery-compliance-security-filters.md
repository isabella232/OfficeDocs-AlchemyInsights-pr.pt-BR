---
title: Nenhum resultado retornado durante a Pesquisa/Exportação de Conteúdo
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101254"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nenhum resultado retornado durante a Pesquisa/Exportação de Conteúdo

Se você estiver enfrentando problemas com os seguintes cenários de Descoberta eDiscovery:

- Pesquisa/Exportação de Conteúdo não retorna dados ou dados inesperados
- Falha na Pesquisa ou Exportação de DescobertaSQuisuportada

Isso pode ser devido a determinados Filtros de Segurança de Conformidade que foram configurados por um Administrador específico e não foram comunicados a todos os Administradores.

Para resolver isso, verifique se há algum Filtro de Segurança de Conformidade que possa estar causando esses problemas:

1. Conexão o Powershell do Centro de Conformidade e Segurança
2. Execute os seguintes comandos:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obter informações adicionais sobre filtros de segurança de conformidade, consulte [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
