---
title: Alterar as configurações de limitação do EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075885"
---
# <a name="changing-ews-throttling-settings"></a>Alterar as configurações de limitação do EWS

Execute nosso teste automatizado, que permitirá modificar a política de limitação do EWS durante a migração. Observe que, mesmo depois de executado, as importações do EWS ainda serão limitadas a 150 MB por 5 minutos por caixa de correio; para alcançar velocidades de transferência de migração mais altas, migre mais usuários simultaneamente.

Observe que as alterações da política de limitação de EWS não afetam os seguintes tipos de migração (utilizando ferramentas da Microsoft): Híbrido, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Pasta Pública ou o Serviço de importação de PST.