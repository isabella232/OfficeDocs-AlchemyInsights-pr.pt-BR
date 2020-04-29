---
title: Criptografia com regras de transporte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915011"
---
# <a name="encryption-with-transport-rules"></a>Criptografia com regras de transporte

No [Centro de Administração do Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), você pode usar os recursos da Criptografia de Mensagens do Office (OME) em suas regras de fluxo de emails para disparar a criptografia de mensagens. Escolha a opção **Aplicar Criptografia de Mensagens e proteção de direitos do Office 365** na condição de Regra de Transporte.

- Para obter mais informações, confira [Definir regra de fluxo de email para criptografia](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- No Powershell, use o cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e defina o parâmetro *ApplyOME* como $true.
