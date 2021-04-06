---
title: Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590260"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows

A Área de Trabalho Virtual do Windows (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros por meio de uma única interface. Esta ferramenta registra informações relacionadas a diagnósticos sempre que a WVD for utilizada por alguém a quem foi atribuído uma função WVD. Cada log contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e as informações sobre o locatário e o usuário. A Análise de Log do Azure pode ser configurada para capturar o log de atividades criado pela ferramenta de diagnóstico seguindo estas etapas:

1. Crie um espaço de trabalho de Análise de Log com o [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Conectar computadores Windows ao Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenha a ID do espaço de trabalho e a chave primária de seu espaço de trabalho. O assistente de configuração precisa destas informações para configurar corretamente o agente e garantir que ele possa se comunicar com o Azure Monitor.

1. [Enviar dados de diagnóstico para o seu espaço de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284). Você pode enviar dados de diagnóstico do seu locatário WVD para a Análise de Log do seu espaço de trabalho.

1. [Identificar e diagnosticar](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas internos ou externos em relação à WVD.

Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para WVD, consulte Usar a Análise de Log para o recurso de diagnóstico.