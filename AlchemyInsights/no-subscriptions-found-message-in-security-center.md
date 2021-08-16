---
title: Nenhuma mensagem de assinatura encontrada na Central de Segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 24b9a7d3e8106c7357f14a00ecb192af4644257577a9549620b6e8b11b6f90d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097438"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nenhuma mensagem de assinatura encontrada na Central de Segurança

Se, ao acessar a Central de Segurança do Microsoft Defender, você receber uma mensagem "Nenhuma assinatura encontrada", isso significa que o Azure Active Directory (AAD) usado para fazer logon do usuário no portal não tem uma licença do Microsoft Defender ATP.  

As licenças do Windows E5 e do Office E5 são licenças separadas.

Abra um caso de suporte se a licença foi adquirida, mas não provisionada para esta instância do AAD. Ou você tem: <br/>
-   Um possível problema de provisionamento de licença.<br/>
-   Você inadvertidamente provisionou a licença para um Microsoft AAD diferente daquele usado para autenticação no serviço.