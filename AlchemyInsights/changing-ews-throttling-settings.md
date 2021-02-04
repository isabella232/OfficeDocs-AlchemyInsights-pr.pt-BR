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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="45e44-102">Alterar as configurações de limitação do EWS</span><span class="sxs-lookup"><span data-stu-id="45e44-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="45e44-103">Execute nosso teste automatizado, que permitirá modificar a política de limitação do EWS durante a migração.</span><span class="sxs-lookup"><span data-stu-id="45e44-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="45e44-104">Observe que, mesmo depois de executado, as importações do EWS ainda serão limitadas a 150 MB por 5 minutos por caixa de correio; para alcançar velocidades de transferência de migração mais altas, migre mais usuários simultaneamente.</span><span class="sxs-lookup"><span data-stu-id="45e44-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="45e44-105">Observe que as alterações da política de limitação de EWS não afetam os seguintes tipos de migração (utilizando ferramentas da Microsoft): Híbrido, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Pasta Pública ou o Serviço de importação de PST.</span><span class="sxs-lookup"><span data-stu-id="45e44-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>