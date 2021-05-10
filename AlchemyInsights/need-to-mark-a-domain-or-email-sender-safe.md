---
title: Precisa marcar um remetente de domínio ou e-mail como seguro?
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
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286668"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Precisa marcar um remetente de domínio ou e-mail como seguro?

- O uso de **listas de remetentes seguros não é recomendado**, pois abre sua organização a ataques de spam, phishing e falsificação.
- No entanto, se houver uma necessidade comercial, **recomendamos** usar **[Regras de fluxo de e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para isso. Nossa orientação garante a autenticação do remetente (verifica se o domínio de envio não está sendo falsificado). **Observação**: não recomendamos o gerenciamento de falsos positivos usando listas de remetentes seguros, pois exceções à filtragem de spam podem abrir sua organização a ataques de segurança. Se seus usuários receberem mensagens marcadas incorretamente como spam ou lixo eletrônico, **[Relate as mensagens e arquivos à Microsoft.](https://protection.office.com/reportsubmission)**.
- Remetentes Seguros no Outlook, lista de remetentes Permitidos ou lista de domínios permitidos nas políticas anti-spam **devem ser evitados** porque os remetentes ignoram toda a proteção contra spam, falsificação e phishing, e autenticação de remetente (SPF, DKIM, DMARC). Este método é melhor usado apenas para testes temporários.
- A validação de que um determinado e-mail ignorou a avaliação antispam pode ser feita verificando o cabeçalho da mensagem “X-Forefront-Antispam-Report" (SFV: SFE, SFV: SKA, SFV: SKN), consulte **[Cabeçalhos de mensagens antispam](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Como a Microsoft deseja manter nossos clientes [seguros por padrão](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), algumas substituições de locatários não serão aplicadas para malware e phishing de alta confiança. Essas substituições incluem: o   Listas de remetentes permitidos ou listas de domínios permitidos (políticas anti-spam) o   Remetentes seguros do Outlook o   Lista de Permissões de IP (filtragem da conexão) 
- A única substituição que permite que mensagens de phishing de alta confiança contornem a filtragem são as regras de fluxo de correio do Exchange (também conhecidas como regras de transporte). Para usar regras de fluxo de email para ignorar a filtragem, consulte **[Usar regras de fluxo de email para definir o nível de confiança de spam (SCL) nas mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.