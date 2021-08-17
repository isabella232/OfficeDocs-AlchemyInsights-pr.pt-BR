---
title: Solucionar Problemas de Eventos do E-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105340"
---
# <a name="troubleshooting-events-from-email"></a>Solucionar Problemas de Eventos do E-mail

1. Verifique se o recurso está habilitado para a caixa de correio: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Em seguida, examine os logs de "Eventos de E-mail" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Nos logs de 'Eventos de E-mail', localize o InternetMessageId que corresponde ao item na caixa de correio.  

4. O TrustScore determina se o item é adicionado ou não. Os eventos só serão adicionados se o TrustScore = "Trusted".

O TrustScore é determinado pelas propriedades SPF, Dkim ou Dmarc, que estão no Cabeçalho da Mensagem.

Para exibir estas propriedades:

**Área de trabalho do Outlook**

- Abra o item
- Arquivo -> Propriedades -> Cabeçalhos de Internet

ou

**MFCMapi**

- Navegue até o item na caixa de entrada
- Procure PR_TRANSPORT_MESSAGE_HEADERS_W

Essas propriedades são determinadas e gravadas durante o transporte e o roteamento. Para obter mais soluções de problemas, talvez seja necessário acompanhar junto ao Suporte de Transporte sobre as falhas no SPF, DKIM e.ou DMARC.