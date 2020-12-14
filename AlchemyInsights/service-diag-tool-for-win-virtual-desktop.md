---
title: Ferramenta de diagnóstico de serviço para área de trabalho virtual do Windows
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665810"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para área de trabalho virtual do Windows

A área de trabalho virtual do Windows (WVD) oferece uma ferramenta de diagnóstico que permite que os administradores identifiquem erros através de uma única interface. Esta ferramenta registra informações relacionadas a diagnóstico sempre que o WVD é usado por alguém que atribui uma função de WVD. Cada log contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e as informações sobre o locatário e o usuário. A análise de logs do Azure pode ser configurada para capturar o log de atividades criado pela ferramenta de diagnóstico. Veja como:

1. Crie um espaço de trabalho da análise de logs com o [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Conectar computadores Windows ao Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obter a ID do espaço de trabalho e a chave primária do seu espaço de trabalho. O assistente de instalação precisa dessas informações para configurar corretamente o agente e para garantir que ele possa se comunicar com o Azure monitor.
1. [Enviar dados de diagnósticos por push para seu espaço de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284). Você pode enviar dados de diagnóstico do seu locatário do WVD para a análise de logs do seu espaço de trabalho.
1. [Identificar e diagnosticar problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos ou externos em relação ao WVD.

Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para o WVD, confira [usar a análise de logs para o recurso de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2128084).
