---
title: Criar um grupo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929293"
---
# <a name="create-a-group"></a>Criar um grupo

Este tópico descreve a criação de grupo.

**Permissão para criar um grupo**

Certifique-se de que você está autorizado a criar um novo grupo. Os administradores globais podem desabilitar a criação de grupos no portal do Azure ou no Painel de Acesso. Talvez você precise de um administrador para criar o novo grupo para você ou para lhe dar as permissões apropriadas.

**Gerenciar permissões de criação de grupo**

1. Os administradores globais podem gerenciar permissões de criação de grupo (por motivos relacionados à segurança) ou grupos Office 365 criados no portal do Azure ou no Painel de Acesso, escolhendo "Os usuários podem criar grupos de segurança em portais do Azure" ou "Os usuários podem criar grupos Office 365 em portais do Azure" em Todos os grupos   >  **Gerais (Configurações)**.
2. Você também pode restringir a criação de grupo para selecionar um grupo de usuários se tiver uma Azure Active Directory P1 Premium licença.

**Desabilitando a notificação de boas-vindas para novos membros Office 365 grupo**

A notificação de boas-vindas enviada aos usuários que são adicionados Office 365 grupos pode ser desabilitada definindo **UnifiedGroupWelcomeMessageEnabled** como False no Powershell. Saiba mais sobre essa configuração [aqui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

