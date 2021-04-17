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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818024"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="10e10-102">Alterar as configurações de limitação do EWS</span><span class="sxs-lookup"><span data-stu-id="10e10-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="10e10-103">Execute nosso teste automatizado, que permitirá modificar a política de limitação do EWS durante a migração.</span><span class="sxs-lookup"><span data-stu-id="10e10-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="10e10-104">Observe que, mesmo depois de executado, as importações do EWS ainda serão limitadas a 150 MB por 5 minutos por caixa de correio; para alcançar velocidades de transferência de migração mais altas, migre mais usuários simultaneamente.</span><span class="sxs-lookup"><span data-stu-id="10e10-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="10e10-105">Observe que as alterações da política de limitação de EWS não afetam os seguintes tipos de migração (utilizando ferramentas da Microsoft): Híbrido, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Pasta Pública ou o Serviço de importação de PST.</span><span class="sxs-lookup"><span data-stu-id="10e10-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>