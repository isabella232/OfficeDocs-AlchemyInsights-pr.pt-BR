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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813676"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erro "Houve um erro ao validar o token de acesso" durante a integração do Desktop Analytics

Esse erro normalmente é observado quando o token de autenticação expira. Normalmente, atualizar a página atualiza o token. No entanto, esse problema pode persistir se houver alguma política de Acesso Condicional aplicada à conta que está sendo usada no Desktop Analytics. Você pode revisar os logs de login do Azure AD no Portal do Azure para ver se há alguma falha de login para a conta que está sendo usada para integração do Desktop Analytics.

Para obter mais informações sobre o Acesso Condicional, visite [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).