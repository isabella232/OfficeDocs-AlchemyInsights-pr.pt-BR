---
title: Retransmitir emails no Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117971"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurar um dispositivo multifuncional ou aplicativo para enviar email

Saiba mais sobre as opções e etapas necessárias em [Como configurar um dispositivo ou aplicativo multifuncional para enviar emails usando o Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Se você tem um dispositivo ou aplicativo que recentemente parou de funcionar, as questões mais comuns são:

- **Autenticação de erros relacionados ao uso da submissão de clientes SMTP Auth** Recentemente fizemos algumas alterações relacionadas ao funcionamento da Autenticação SMTP. Para mais informações sobre como resolver problemas, veja a seção de autenticação sem sucesso de [Corrigir problemas com impressoras, scanners e aplicativos LOB que enviam emails usando Microsoft 365 ou Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Aceitamos somente a versão TLS 1.2 enquanto fazemos uma conexão segura com o Office 365** Se você estiver usando uma conexão segura (TLS), certificar de que seu dispositivo de aplicação suporta o TLS 1.2. Para mais informações, veja [Preparação para o TLS 1.2 no Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Para outras questões e soluções, veja [Correção de problemas com impressoras, scanners e aplicativos LOB que enviam emails usando Microsoft 365 ou Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Para ver os dispositivos afetados, vá para o relatório [SMTP Auth Clients](https://protection.office.com/mailflow/dashboard).

**Nota**: Exchange Online não acomoda cenários de correio a granel. Para enviar emails comerciais em massa (por exemplo, boletins informativos de clientes), você deve usar provedores terceirizados especializados nestes serviços.
