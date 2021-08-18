---
title: Importar e Exportar do Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: b365921d3ca64e8ad4bd3891e11add8043b2a903
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329814"
---
# <a name="import-and-export-from-yammer"></a>Importar e Exportar do Yammer

**Importação**

As opções de importação do usuário variam dependendo se a sua rede do Yammer está ou não no [Modo Nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).

- **Modo não nativo**: os usuários podem ser importados para grupos usando o [Adicionar do Catálogo de Endereços](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite de 100 usuários) nas configurações do grupo ou para a rede usando o [Atualização em Massa](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) no Administrador de Rede.
- **Modo Nativo**: as operações de associação a um grupo e de associação de rede devem ser executadas no [Portal de administração do Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Portal do Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ou usando outra opção do Azure AD. As redes no Modo Nativo não têm mais acesso à Atualização em Massa e a outros recursos herdados.

    **Importante**: o Yammer nunca teve suporte para a importação de conteúdo dentro do Administrador de Rede mesmo quando o recurso Exportação de Dados era usado em outra rede. O conteúdo pode ser repostado por soluções de parceiros ou pelas APIs REST do Yammer.

**Exportar**

[Exportar Dados de Rede dentro do Administrador de Rede](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite a exportação de conteúdo de redes do Yammer, incluindo mensagens e arquivos. Os anexos podem ser extremamente grandes e farão com que as exportações demorem muito para serem concluídas. Recomendamos que as redes ativas sejam exportadas usando a [API de Exportação de Dados](https://developer.yammer.com/docs/data-export-api) em blocos por dia ou por semana. O Suporte da Microsoft não fornece scripts personalizados para essa finalidade.

Uma [Exportação de GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separada existe para exportar o conteúdo para um usuário individual.