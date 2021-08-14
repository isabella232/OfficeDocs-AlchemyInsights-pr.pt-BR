---
title: Configurações de SMTP para o serviço de email do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 261695a0bf736a51514df50c0ad66aaab5b50edb
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603223"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Configurações de SMTP para o serviço de email do Microsoft 365

Estas são as configurações de SMTP para os serviços de email do Microsoft 365:

**Server**: smtp.office365.com </br>
**Porta**: 587 </br>
**Criptografia**: STARTTLS (Apenas a versão TLS 1.2 é atualmente compatível. Certifique-se de que seu aplicativo ou dispositivo seja compatível com o TLS 1.2) </br>
**Nome de usuário**: Seu endereço do Office 365 (por exemplo, exemplo@seudominio.com) </br>
**Senha**: A sua senha do Office 365 </br>
**Autenticação**: Obrigatória </br>
**Limites de envio**: 10.000 emails por dia </br>

Para configurações de POP e IMAP, consulte [configurações de POP, IMAP e SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Para saber mais sobre as suas opções para retransmitir email usando o Microsoft 365 e as etapas, consulte [Como configurar um dispositivo ou aplicativo multifuncional para enviar emails usando o Microsoft 365 ou Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).