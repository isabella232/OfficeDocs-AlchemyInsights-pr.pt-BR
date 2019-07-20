---
title: Pesquisa de conteúdo sem resultados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800170"
---
# <a name="no-results-from-content-searchexports"></a>Nenhum resultado de pesquisa/exportação de conteúdo

Problemas de pesquisa/exportação de conteúdo que não retornam dados podem ser devido ao certo filtro de segurança de conformidade que foi configurado por um administrador específico e não está se comunicando com todos os administradores.

Para resolver isso, verifique se há algum filtro de segurança de conformidade que possa estar causando o seguinte:
1. Conectar-se ao PowerShell do centro de conformidade e segurança
2. Execute o seguinte comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org