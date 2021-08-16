---
title: Alterar as configurações de limitação do EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968365"
---
# <a name="changing-ews-throttling-settings"></a>Alterar as configurações de limitação do EWS

Execute nosso teste automatizado, que permitirá modificar a política de limitação do EWS durante a migração. Observe que, mesmo depois de executado, as importações do EWS ainda serão limitadas a 150 MB por 5 minutos por caixa de correio; para alcançar velocidades de transferência de migração mais altas, migre mais usuários simultaneamente.

Observe que as alterações da política de limitação de EWS não afetam os seguintes tipos de migração (utilizando ferramentas da Microsoft): Híbrido, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Pasta Pública ou o Serviço de importação de PST.