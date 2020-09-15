---
title: Pesquisa de conteúdo sem resultados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680635"
---
# <a name="no-results-from-content-searchexports"></a>Nenhum resultado de pesquisa/exportação de conteúdo

Problemas de pesquisa/exportação de conteúdo que não retornam dados podem ser devido ao certo filtro de segurança de conformidade que foi configurado por um administrador específico e não está se comunicando com todos os administradores.

Para resolver isso, verifique se há algum filtro de segurança de conformidade que possa estar causando o seguinte:
1. Conectar-se ao PowerShell do centro de conformidade e segurança
2. Execute o seguinte comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org