---
title: 2681 do simulador de ataque no Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759207"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de ataque no Microsoft 365

- Você está faltando no simulador de ataques? O simulador de ataque requer o **office 365 Advanced Threat Protection Plan 2 (plano ATP 2)** ou o **Office 365 Enterprise E5**. O simulador de ataques **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (plano ATP 1), Office 365 Enterprise E3 ou qualquer aplicativo do Microsoft 365 para assinaturas de negócios.

- A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e a autenticação multifator (MFA). Para obter mais informações sobre os requisitos de simulador de ataques, consulte [Este tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Considerações importantes sobre simulações de ataque de **senha de força bruta** :

  - Se a conta de destino tiver a MFA habilitada e a senha tiver sido adivinhada corretamente, a conta não será mostrada como comprometida (o segundo fator de autenticação estará incompleto).

  - O arquivo de senha não pode ter mais de 10 MB. Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.

- Coisas importantes que você deve saber sobre as simulações de conexões de **spear phishing** :

  - Por design, você não pode fornecer um valor personalizado para a **URL do servidor de logon de phishing**.

  - Se um destinatário usar o [suplemento habilitar o relatório de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (pois esse é um ataque simulado).

- Relatórios: após a conclusão do ataque simulado, você pode clicar em **detalhes do ataque** para ver o relatório.

- Para obter instruções detalhadas e novos recursos no simulador de ataques, consulte [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
