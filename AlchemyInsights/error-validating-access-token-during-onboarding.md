---
title: Ocorreu um erro ao validar o erro de token de acesso durante a integração de análise da área de trabalho
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741112"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erro "ocorreu um erro ao validar o token de acesso" durante a integração da análise de desktop

Esse erro normalmente é observado quando o token de autenticação expira. Normalmente, a atualização da página atualiza o token. No entanto, esse problema pode persistir se houver políticas de acesso condicional aplicadas à conta que está sendo usada para a análise de desktop integrado. Você pode revisar os logs de entrada do Azure AD no portal do Azure para ver se há falhas de logon para a conta que está sendo usada para a integração do desktop Analytics.

Para obter mais informações sobre acesso condicional, visite [Plan Your Conditional Access Deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).