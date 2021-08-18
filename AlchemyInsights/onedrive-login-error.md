---
title: OneDrive erro de logon AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112900"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive erro de logon AADSTS50011

Se você receber um erro "AADSTS50011: A URL de resposta especificada na solicitação não corresponderá à resposta" ao entrar no aplicativo OneDrive, verifique o seguinte:

Sua OneDrive versão precisa ser igual ou maior que a versão 20.052.XXXX.XXXX. Para verificar sua versão, clique no ícone azul OneDrive na área de notificação, selecione **Ajuda & Configurações > Configurações > Sobre**.

Sua rede pode bloquear o tráfego para **g.live.com** e **oneclient.sfx.ms**. Se esse tráfego estiver bloqueado, OneDrive não poderá se atualizar. Trabalhe com o administrador de rede para garantir que você tenha acesso a essas URLs. [Esses pontos de extremidade devem](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) ser acessíveis para clientes que usam Microsoft 365 planos.

Se você precisar obter manualmente uma versão atual do OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
