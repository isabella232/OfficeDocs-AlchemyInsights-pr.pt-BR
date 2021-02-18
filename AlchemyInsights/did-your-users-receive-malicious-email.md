---
title: Seus usuários recebem emails mal-intencionados
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291780"
---
# <a name="did-your-users-receive-malicious-email"></a>Os seus usuários recebem emails mal-intencionados?

- Agora você pode facilmente relatar para A Microsoft usando os [Envios de Administradores no Centro de Conformidade e Segurança](https://sip.protection.office.com/reportsubmission).

As mensagens enviadas em [envios do administrador](https://sip.protection.office.com/reportsubmission) são verificadas e os seguintes resultados são exibidos no menu desdobrável **detalhes**:

- Se houve falha na autenticação do email do remetente no momento da entrega.
- Informações sobre quaisquer acessos à política que possam ter afetado ou substituído o veredicto de uma mensagem.
- Resultados de detonação atuais para ver se os URLs ou arquivos contidos na mensagem eram maliciosos ou não.
- Feedback dos avaliadores

Se uma substituição for encontrada, a nova varredura deve ser concluída em alguns minutos. Se não houvesse problema na autenticação do email ou se a entrega não fosse afetada por uma modificação, o feedback dos avaliadores poderia levar até um dia.

Se você discordar do veredicto final em uma mensagem, URL ou arquivo (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para nova varredura. As chances são altas de que o veredicto mude depois de enviar a mensagem novamente.

Enquanto isso, você pode remover e-mails maliciosos das caixas de entrada dos usuários, seguindo as instruções [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Os clientes com Microsoft Defender para Office 365 podem:
    - use [Threat Explorer para Localizar e Excluir emails Suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [use links seguros para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a um URL malicioso
    - rastrear usuários que clicaram e acessaram URLs maliciosos: [View URL de phishing e dados de veredicto de cliques](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - manualmente [iniciar uma Investigação Automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Você também pode se proteger contra arquivos e URLs maliciosos, seguindo as instruções em [Proteção contra URLs e arquivos maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).