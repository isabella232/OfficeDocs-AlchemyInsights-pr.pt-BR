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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057990"
---
# <a name="no-results-from-content-searchexports"></a>Nenhum resultado da Pesquisa de Conteúdo/Exportações

Problemas com a Pesquisa de Conteúdo/Exportações que não retornam dados podem ser devido a determinado Filtro de Segurança de Conformidade que foi configurado por um administrador específico e não os comunica a todos os administradores.

Para resolver isso, verifique se há algum Filtro de Segurança de Conformidade que possa estar causando isso:
1. Conexão o Powershell do Centro de Conformidade e Segurança
2. Execute os seguintes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org