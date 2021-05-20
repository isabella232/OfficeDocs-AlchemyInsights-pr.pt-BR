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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544096"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nenhuma mensagem de assinatura encontrada na Central de Segurança

Se, ao acessar a Central de Segurança do Microsoft Defender, você receber uma mensagem "Nenhuma assinatura encontrada", isso significa que o Azure Active Directory (AAD) usado para fazer logon do usuário no portal não tem uma licença do Microsoft Defender ATP.  

As licenças do Windows E5 e do Office E5 são licenças separadas.

Abra um caso de suporte se a licença foi adquirida, mas não provisionada para esta instância do AAD. Ou você tem: <br/>
-   Um possível problema de provisionamento de licença.<br/>
-   Você inadvertidamente provisionou a licença para um Microsoft AAD diferente daquele usado para autenticação no serviço.