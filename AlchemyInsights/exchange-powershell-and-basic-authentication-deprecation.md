---
title: Reprovação de autenticação básica e Exchange PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069232"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Reprovação de autenticação básica e Exchange PowerShell

Para obter as informações mais recentes sobre como se conectar ao Exchange Online PowerShell sem o uso da Autenticação Básica, [acesse esse link](https://aka.ms/exops-docs). O módulo PowerShell V2 não usa a autenticação básica.

Observe que a Autenticação Básica ainda deve estar habilitada em sua máquina cliente.
O novo módulo do PowerShell v2 usa Autenticação Moderna para estabelecer conexão para habilitar todos os Cmdlets V2 baseados em REST. Além de cmdlets V2, ela também permite que você acesse Cmdlets mais antigos do PowerShell Remoto (RPS) que exigem que uma sessão do PowerShell Remoto seja estabelecida. O estabelecimento de uma sessão RPS no computador com Windows exige que o WinRM BasicAuth esteja habilitado no computador cliente, mesmo que o módulo use o mecanismo de Autenticação Moderna para se autenticar no serviço. O pipeline de Autenticação Básica do WinRM é usado para transportar tokens de Autenticação Moderna. Se a Autenticação Básica do WinRM estiver desabilitada na máquina cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets mais antigos do RPS não funcionarão).
