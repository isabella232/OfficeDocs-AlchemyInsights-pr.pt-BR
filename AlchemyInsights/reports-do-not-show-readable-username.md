---
title: Relatórios no Centro de administração do Microsoft 365 não mostram nome de usuário legível
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "9008619"
ms.openlocfilehash: 1741aab633b28a9c991a3e4a972f85a67c26705e
ms.sourcegitcommit: 1761960d03b3df7783b744ee539a7e6dbabae90c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/03/2021
ms.locfileid: "58884040"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Relatórios no Centro de administração do Microsoft 365 não mostram nome de usuário legível

Os relatórios no Centro de administração do Microsoft 365 não mostram nomes de usuário, mas, em vez disso, valores alfanuméricos, como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este é o comportamento esperado e foi comunicado no Message Center (MC275344, publicado em 3 de agosto de 2021). 

Os administradores globais podem reverter essa alteração para seu locatário e mostrar informações identificáveis do usuário se as práticas de privacidade de sua organização permitirem. Para reverter a alteração para o inquilino:

1. No centro de administração, acesse **Configurações** > **Configurações da organização** > **Serviços** e selecione **Relatórios**. 
1. Em **Escolher como mostrar as informações do usuário**, selecione **Mostrar informações identificáveis do usuário nos relatórios** e execute novamente o relatório.