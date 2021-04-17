---
title: Pesquisa de Conteúdo Sem Resultados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816836"
---
# <a name="no-results-from-content-searchexports"></a>Nenhum resultado da Pesquisa de Conteúdo/Exportações

Problemas com a Pesquisa de Conteúdo/Exportações que não retornam dados podem ser devido a determinado Filtro de Segurança de Conformidade que foi configurado por um administrador específico e não os comunica a todos os administradores.

Para resolver isso, verifique se há algum Filtro de Segurança de Conformidade que possa estar causando isso:
1. Conectar-se ao Powershell do Centro de Segurança e Conformidade
2. Execute os seguintes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org