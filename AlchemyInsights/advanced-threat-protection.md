---
title: Obter o Microsoft Defender para Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 61236d1e0174248cdb49284d6c6c7d49df51e7e9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315066"
---
# <a name="microsoft-defender-for-office-365"></a>Microsoft Defender para Office 365

- Cofre Anexos, Cofre links e anti-phishing fazem parte do Microsoft Defender para Office 365. Enterprise E5, Education A5 e Microsoft 365 Business Premium incluem o Microsoft Defender para Office 365. Todos os outros planos exigem um complemento do Microsoft Defender para Office 365 assinatura.

- Você precisa atribuir as licenças apropriadas para proteger seus usuários pelo Microsoft Defender para Office 365. Consulte [Adicionar usuários e atribuir licenças](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) ao mesmo tempo para obter instruções sobre como aplicar licenças em massa aos usuários.

- Administradores globais ou administradores de segurança podem acessar o Microsoft Defender para Office 365 recursos no portal Microsoft 365 Defender na seção **Email & de** colaboração Políticas & \> **regras** Políticas \> **de ameaça.**

- Cofre As políticas de anexos e Cofre links podem ser escopo para domínios específicos, membros do grupo ou usuários individuais. Você também pode especificar exceções para Cofre anexos e Cofre links com base no domínio, associação de grupo ou usuários individuais.

- Não há nenhuma política de Cofre de anexos padrão que proteja mensagens de email. Você precisa criar [uma política para a](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-attachments-policies) proteção Cofre Anexos no email.

  Cofre Os anexos para SharePoint, OneDrive e Microsoft Teams estão habilitados ou desabilitados globalmente e não exigem políticas Cofre Attachments. Para obter mais informações, [consulte Cofre Attachments for SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/mdo-for-spo-odb-and-teams).

- Não há nenhuma política de Cofre links padrão que proteja mensagens de email ou Microsoft Teams. Você precisa criar [uma política para a](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies) proteção Cofre Links no email e Teams.

  Cofre A proteção de links para Office 365 aplicativos é aplicada a todos os usuários na organização licenciados para o Defender para Office 365, independentemente de os usuários estar incluídos em políticas Cofre Links ativos ou não. Para obter mais informações, [consulte Cofre Configurações de Links para Office 365 aplicativos](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links#safe-links-settings-for-office-365-apps).
