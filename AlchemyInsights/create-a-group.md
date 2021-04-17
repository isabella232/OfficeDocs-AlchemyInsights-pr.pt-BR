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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816332"
---
# <a name="create-a-group"></a>Criar um grupo

Este tópico descreve a criação de grupo.

**Permissão para criar um grupo**

Certifique-se de que você está autorizado a criar um novo grupo. Os administradores globais podem desabilitar a criação de grupos no portal do Azure ou no Painel de Acesso. Talvez você precise de um administrador para criar o novo grupo para você ou para lhe dar as permissões apropriadas.

**Gerenciar permissões de criação de grupo**

1. Os administradores globais podem gerenciar permissões de criação de grupo (por motivos relacionados à segurança) ou grupos do Office 365 criados no portal do Azure ou no Painel de Acesso, escolhendo "Os usuários podem criar grupos de segurança em portais do Azure" ou "Os usuários podem criar grupos do Office 365 em portais do Azure" em Todos os grupos  >  **Gerais (Configurações)**.
2. Você também pode restringir a criação de grupo para selecionar um grupo de usuários se tiver uma licença do Azure Active Directory P1 Premium.

**Desabilitando a notificação de boas-vindas para novos membros do grupo do Office 365**

A notificação de boas-vindas enviada aos usuários que são adicionados aos grupos do Office 365 pode ser desabilitada definindo **UnifiedGroupWelcomeMessageEnabled** como False no Powershell. Saiba mais sobre essa configuração [aqui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

