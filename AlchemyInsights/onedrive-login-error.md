---
title: Erro de logon do OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947471"
---
# <a name="onedrive-login-error-aadsts50011"></a>Erro de logon do OneDrive AADSTS50011

Se você receber uma mensagem de erro "AADSTS50011: a URL de resposta especificada na solicitação não corresponde à resposta" ao entrar no aplicativo OneDrive, verifique o seguinte:

Sua versão do OneDrive precisa ser igual ou superior à versão 20.052. XXXX. XXXX. Para verificar sua versão, clique no ícone azul do OneDrive na área de notificação, selecione **ajuda & configurações > configurações > sobre**.

Sua rede pode bloquear o tráfego para o **g.Live.com** e o **oneclient.SFX.ms**. Se esse tráfego estiver bloqueado, o OneDrive não poderá se atualizar. Trabalhe com seu administrador de rede para garantir que você tenha acesso a essas URLs. [Esses pontos de extremidade](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devem ser acessíveis para clientes que usam o Microsoft 365 Plans.

Se você precisar obter uma versão atual do OneDrive, acesse [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
