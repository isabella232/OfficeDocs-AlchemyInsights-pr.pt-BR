---
title: Alertas ausentes da guia Alertas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362352"
---
# <a name="alerts-missing-from-alerts-tab"></a>Alertas ausentes da guia Alertas

A **guia Alertas** funciona com base na configuração e políticas ativadas do portal de Governança de Aplicativos em seu locatário. As políticas in-locar na Governança de Aplicativos também devem ser ativadas para permitir que os sinais fluam para a **guia Alertas.** 

Confirme se o alerta foi gerado:

1. Vá para Políticas de [governança](https://compliance.microsoft.com/m365appprotection?viewid=policies) de aplicativos e confirme se você criou pelo menos uma política Ativa ou Auditoria.

1. Selecione a política e, em seguida, seleect **Edit** no painel de sobrevoos. 

1. Verifique a configuração da política para confirmar se um alerta deve ter sido gerado com base em um evento de política iniciado há mais de 24 horas.

Para obter mais informações sobre alertas na Governança de Aplicativos, consulte Começar a detectar e [remediar](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)ameaças de aplicativos.