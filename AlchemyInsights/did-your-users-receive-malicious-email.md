---
title: Seus usuários recebem emails mal-intencionados
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893391"
---
# <a name="did-your-users-receive-malicious-email"></a>Os seus usuários recebem emails mal-intencionados?

Agora você pode relatar o email mal-intencionado à Microsoft usando [Envios no portal do Microsoft 365 Defender](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

As mensagens enviadas em [Envios do administrador](https://security.microsoft.com/reportsubmission?viewid=admin) são verificadas e os seguintes resultados são exibidos no submenu de detalhes:

- Se houve falha na autenticação do email do remetente no momento da entrega.
- Informações sobre quaisquer acessos à política que possam ter afetado ou substituído o veredicto de uma mensagem.
- Resultados de detonação atuais para ver se os URLs ou arquivos contidos na mensagem eram maliciosos ou não.
- Feedback dos avaliadores

Se uma substituição for encontrada, a nova varredura deve ser concluída em alguns minutos. Se não houvesse problema na autenticação do email ou se a entrega não fosse afetada por uma modificação, o feedback dos avaliadores poderia levar até um dia.

Se você discordar do veredicto final em uma mensagem, URL ou arquivo (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para nova varredura. As chances são altas de que o veredicto mude depois de enviar a mensagem novamente.

Enquanto isso, você pode remover e-mails maliciosos das caixas de entrada dos usuários, seguindo as instruções [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Os clientes com Microsoft Defender para Office 365 podem:
  - Use o [Explorador de ameaças para localizar e excluir emails suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Use Links seguros para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) a uma URL mal-intencionada
  - Acompanhe os usuários que clicaram e acessaram URLs mal-intencionadas: [Exibir URL de phishing e clicar em dados de veredito](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Manualmente, [inicie uma Investigação automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Você também pode se proteger contra arquivos e URLs maliciosos, seguindo as instruções em [Proteção contra URLs e arquivos maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
