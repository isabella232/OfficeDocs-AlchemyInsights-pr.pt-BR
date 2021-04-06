---
title: Identificar problemas da Área de Trabalho Virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590259"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identificar problemas da Área de Trabalho Virtual do Windows

O Diagnóstico da Área de Trabalho Virtual do Windows usa apenas um cmdlet do PowerShell, mas contém vários parâmetros opcionais para ajudar a reduzir e isolar problemas. Para começar: 

1. Baixe e importe o módulo do PowerShell da Área de Trabalho Virtual do Windows. Para obter detalhes, confira [Cmdlets da Área de Trabalho Virtual do Windows para o Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Execute o cmdlet a seguir para entrar em sua conta:
    
    Exemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**OBSERVAÇÃO:** todas as consultas que usam o PowerShell devem incluir os parâmetros -UserName ou -ActivityID. Para saber mais sobre recursos de monitoramento, confira [Análise de logs para o recurso de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).

Para filtrar as atividades de diagnóstico por usuário, execute o seguinte cmdlet:

Exemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Há uma lista de filtros que você pode executar para diagnosticar problemas. Para saber mais sobre problemas de diagnóstico, confira [Identificar e diagnosticar problemas da Área de Trabalho Virtual do Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Para saber mais sobre erros comuns, confira [Cenários de erros comuns](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
