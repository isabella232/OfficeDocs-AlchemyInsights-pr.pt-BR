---
title: Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052374"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows

A Área de Trabalho Virtual do Windows (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros por meio de uma única interface. Esta ferramenta registra informações relacionadas a diagnósticos sempre que a WVD for utilizada por alguém a quem foi atribuído uma função WVD. Cada log contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e as informações sobre o locatário e o usuário. O Azure Log Analytics pode ser configurado para capturar o log de atividades criado pela ferramenta de diagnóstico. Veja como:

1. Crie um espaço de trabalho de Análise de Log com o [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Conectar computadores Windows ao Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenha a ID do espaço de trabalho e a chave primária de seu espaço de trabalho. O assistente de configuração precisa destas informações para configurar corretamente o agente e garantir que ele possa se comunicar com o Azure Monitor.
1. [Enviar dados de diagnóstico para o seu espaço de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284). Você pode enviar dados de diagnóstico do seu locatário WVD para a Análise de Log do seu espaço de trabalho.
1. [Identifique e diagnostice problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos ou externos em relação ao WVD.

Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para WVD, consulte [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).
