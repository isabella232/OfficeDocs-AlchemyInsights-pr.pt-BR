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
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327802"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Relatórios no Centro de administração do Microsoft 365 não mostram nome de usuário legível

Os relatórios no Centro de administração do Microsoft 365 não mostram nomes de usuário, mas, em vez disso, valores alfanuméricos, como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este é o comportamento esperado e foi comunicado no Message Center (MC275344, publicado em 3 de agosto de 2021). 

Os administradores globais podem reverter essa alteração para seu locatário e mostrar informações identificáveis do usuário se as práticas de privacidade de sua organização permitirem. Para reverter a alteração para o inquilino:

1. No centro de administração, acesse **Configurações** > **Configurações da organização** > [**Serviços**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) e selecione **Relatórios**. 
1. Em **Escolher como mostrar as informações do usuário**, selecione **Mostrar informações identificáveis do usuário nos relatórios** e execute novamente o relatório.