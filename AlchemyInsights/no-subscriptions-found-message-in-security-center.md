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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768328"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nenhuma mensagem de assinatura encontrada na Central de Segurança

Se, ao acessar a Central de Segurança do Microsoft Defender, você receber uma mensagem "Nenhuma assinatura encontrada", isso significa que o Azure Active Directory (AAD) usado para fazer o logon do usuário no portal não tem uma licença da Proteção Avançada contra Ameaças do Microsoft Defender.  

As licenças do Windows E5 e do Office E5 são licenças separadas.

Abra um caso de suporte se a licença foi adquirida, mas não provisionada para esta instância do AAD. Ou você tem: <br/>
-   Um possível problema de provisionamento de licença.<br/>
-   Você inadvertidamente provisionou a licença para um Microsoft AAD diferente daquele usado para autenticação no serviço.