---
title: Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806423"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios

**Sintoma**

Os usuários não conseguem abrir relatórios. "Algo deu errado. Verifique detalhes técnicos para obter mais detalhes."

**Causa**

Os relatórios não serão carregados no UCI com o erro "O descritor de formulário é nulo ou não definido". Os relatórios na UCI ainda exigem caixas de diálogo herdadas, nesse caso, o sistema do cliente precisa ter o *allowlegacydialogsembedding* habilitado.

**Solução**

1. Acesse **Configurações > Administração > Configurações do Sistema > Guia Geral**.

2. Configure "Habilitar a incorporação de determinadas caixas de diálogo herdadas no cliente do navegador da Interface Unificada" para **Sim**.
