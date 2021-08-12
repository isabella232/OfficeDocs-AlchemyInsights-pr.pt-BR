---
title: Houve um erro ao validar um erro de token de acesso durante a abordagem do Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946603"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erro "Houve um erro ao validar o token de acesso" durante a integração do Desktop Analytics

Esse erro normalmente é observado quando o token de autenticação expira. Normalmente, atualizar a página atualiza o token. No entanto, esse problema pode persistir se houver alguma política de Acesso Condicional aplicada à conta que está sendo usada no Desktop Analytics. Você pode revisar os logs de login do Azure AD no Portal do Azure para ver se há alguma falha de login para a conta que está sendo usada para integração do Desktop Analytics.

Para obter mais informações sobre o Acesso Condicional, visite [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).