---
title: Solucionar problemas de erros de suspensão da Descoberta Eletrônica
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 2a7372c7b20b87c8c774eae4ca4540a3bd19709596405da041eeaa24db310fa7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105376"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Solucionar problemas de erros de suspensão da Descoberta Eletrônica

Enfrentando problemas de suspensão da Descoberta Eletrônica? Considere uma das seguintes práticas recomendadas:

- Verifique o status de distribuição da suspensão.  Se o status estiver **Ativado (Pendente)** ou **Desativado (Pendente)**, aguarde a distribuição de suspensão ser concluída.
- Mescle as atualizações de suspensão da Descoberta Eletrônica em uma única solicitação em massa, ao invés de atualizar a política repetidamente para cada transação.
- Execute Set-CaseHoldPolicy <policyname> –RetryDistribution no Centro de Conformidade e Segurança do Powershell. Para mais detalhes, confira [Conectar-se ao Centro de Conformidade e Segurança do PowerShell](/powershell/exchange/connect-to-scc-powershell).

Para obter as etapas de verificação dessas configurações e as práticas recomendadas adicionais para reduzir e resolver problemas de suspensão da Descoberta Eletrônica, confira [Solucionar problemas de erros de suspensão da Descoberta Eletrônica](/microsoft-365/compliance/hold-distribution-errors).
Para obter informações sobre como solucionar outros problemas comuns da Descoberta Eletrônica, confira [Investigar e solucionar os problemas mais comuns da Descoberta Eletrônica](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
