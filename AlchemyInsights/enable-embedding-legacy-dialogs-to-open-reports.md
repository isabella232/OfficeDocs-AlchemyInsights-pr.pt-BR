---
title: Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814252"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios

**Sintoma**

Os usuários não conseguem abrir relatórios. "Algo deu errado. Verifique detalhes técnicos para obter mais detalhes."

**Causa**

Os relatórios não serão carregados no UCI com o erro "O descritor de formulário é nulo ou não definido". Os relatórios na UCI ainda exigem caixas de diálogo herdadas, nesse caso, o sistema do cliente precisa ter o *allowlegacydialogsembedding* habilitado.

**Solução**

1. Acesse **Configurações > Administração > Configurações do Sistema > Guia Geral**.

2. Configure "Habilitar a incorporação de determinadas caixas de diálogo herdadas no cliente do navegador da Interface Unificada" para **Sim**.
