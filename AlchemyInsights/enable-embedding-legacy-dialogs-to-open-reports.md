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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003377"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios

**Sintoma**

Os usuários não conseguem abrir relatórios. "Algo deu errado. Verifique detalhes técnicos para obter mais detalhes."

**Causa**

Os relatórios não serão carregados no UCI com o erro "O descritor de formulário é nulo ou não definido". Os relatórios na UCI ainda exigem caixas de diálogo herdadas, nesse caso, o sistema do cliente precisa ter o *allowlegacydialogsembedding* habilitado.

**Solução**

1. Acesse **Configurações > Administração > Configurações do Sistema > Guia Geral**.

2. Configure "Habilitar a incorporação de determinadas caixas de diálogo herdadas no cliente do navegador da Interface Unificada" para **Sim**.
