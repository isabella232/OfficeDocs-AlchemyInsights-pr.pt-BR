---
title: Simulador de Ataque 2681 no Microsoft 365
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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065272"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de Ataque no Microsoft 365

- Você está perdendo o Simulador de Ataque? O Simulador de Ataque requer **o Microsoft Defender para Office 365 Plano 2** ou Office 365 Enterprise **E5**. O **Simulador** de Ataque não está incluído no Microsoft Defender para Office 365 Plano 1, Office 365 Enterprise E3 ou qualquer assinatura Microsoft 365 Apps para Pequenos e Médios negócios.

- A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e autenticação multifafatória (MFA). Para obter mais informações sobre os requisitos do Simulador de Ataque, [consulte este tópico](/microsoft-365/security/office-365-security/attack-simulator).

- Coisas importantes a saber sobre **simulações** de ataque de Senha de Força Bruta:

  - Se a conta de destino tiver MFA habilitada e a senha tiver sido adivinhada corretamente, a conta não mostrará como comprometida (o segundo fator de autenticação estará incompleto).

  - O arquivo de senha não pode ser maior do que 10 MB. Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.

- Coisas importantes a saber sobre simulações de **anexação de Phishing** de Lança:

  - Por design, você não pode fornecer um valor personalizado para a URL do servidor **de logon de Phishing.**

  - Se um destinatário usar o complemento [Habilitar](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) a Mensagem de Relatório para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (porque é um ataque simulado).

- Relatórios: depois que o ataque simulado for concluído, você poderá clicar em **Detalhes de** Ataque para ver o relatório.

- Para obter instruções detalhadas e novos recursos no Simulador de Ataques, consulte [Simulador](/microsoft-365/security/office-365-security/attack-simulator)de Ataque em Microsoft 365 .
