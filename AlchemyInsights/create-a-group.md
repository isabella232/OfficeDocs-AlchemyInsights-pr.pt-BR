---
title: Criar um grupo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086201"
---
# <a name="create-a-group"></a>Criar um grupo

Este tópico descreve a criação de grupos.

**Permissão para criar um grupo**

Certifique-se de que você está autorizado a criar um novo grupo. Os administradores globais podem desabilitar a criação de grupos no portal do Azure ou no painel de acesso. Você pode precisar de um administrador para criar o novo grupo ou fornecer as permissões apropriadas.

**Gerenciar permissões de criação de grupo**

1. Os administradores globais podem gerenciar permissões de criação de grupos (por motivos relacionados à segurança) ou grupos do Office 365 criados no portal do Azure ou no painel de acesso, escolhendo "os usuários podem criar grupos de segurança nos portais do Azure" ou "os usuários podem criar grupos do Office 365 no Azure Portals" em **todos os grupos**  >  **gerais (configurações)**.
2. Você também pode restringir a criação de grupo para selecionar um grupo de usuários se você tiver uma licença do Azure Active Directory P1 Premium.

**Desabilitando a notificação de boas-vindas para os novos membros do grupo do Office 365**

A notificação de boas-vindas enviada aos usuários adicionados aos grupos do Office 365 pode ser desabilitada definindo **UnifiedGroupWelcomeMessageEnabled** como false no PowerShell. Saiba mais sobre essa configuração [aqui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

