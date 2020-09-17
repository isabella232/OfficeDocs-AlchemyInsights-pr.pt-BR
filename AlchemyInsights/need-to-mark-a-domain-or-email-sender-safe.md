---
title: Precisa marcar um remetente de domínio ou e-mail como seguro?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803233"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Precisa marcar um remetente de domínio ou e-mail como seguro?

- O uso de **listas de remetentes seguros não é recomendado**, pois abre sua organização a ataques de spam, phishing e falsificação.
- No entanto, se houver uma necessidade comercial, **recomendamos** usar **[Regras de fluxo de e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para isso. Nossa orientação garante a autenticação do remetente (verifica se o domínio de envio não está sendo falsificado). **Observação**: não recomendamos o gerenciamento de falsos positivos usando listas de remetentes seguros, pois exceções à filtragem de spam podem abrir sua organização a ataques de segurança. Se seus usuários receberem mensagens marcadas incorretamente como spam ou lixo eletrônico, **[Relate as mensagens e arquivos à Microsoft.](https://protection.office.com/reportsubmission)**.
- Remetentes seguros no Outlook, lista de remetentes permitidos ou lista de domínios permitidos nas políticas anti-spam **devem ser evitados** porque os remetentes ignoram toda a proteção contra spam, spoof e phishing e autenticação de remetente (SPF, DKIM, DMARC). Esse método é melhor usado apenas para testes temporários.
