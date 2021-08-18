---
title: Corrigir problemas comuns com o Microsoft Defender para Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330048"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Corrigir problemas comuns com o Microsoft Defender para Office 365

Aqui estão algumas soluções para problemas comuns com o Microsoft Defender para Office 365:

- **Atraso da mensagem**:

  Atrasos na entrega de email podem ser causados Cofre verificação de anexos de mensagens. Para obter mais informações, consulte Cofre configurações de política [de anexos.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Relatar resultados falsos positivos ou negativos:**

  Para mais informações, confira [Relatar mensagens e arquivos à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Habilitar Cofre proteção de link**:

  1. No portal Microsoft 365 Defender em , vá para Email & Políticas de Colaboração & Políticas de Ameaças de Regras Cofre Links na <https://security.microsoft.com/>  \>  \>  \>  **seção** Políticas.

     Para ir diretamente para a página **Cofre Links,** use <https://security.microsoft.com/safelinksv2> .

  2. Na página **Cofre Links,** selecione a política clicando no nome da política.
  3. No sobremenu de detalhes exibido, faça uma das seguintes etapas:
     - Para adicionar uma nova política, selecione **+ Criar**. Um assistente será lançado para ajudá-lo a definir suas configurações de política.
     - Para editar uma política existente, selecione a política clicando no nome da política. No sobremenu de detalhes exibido, selecione **Editar** na **seção Configurações de** Proteção.
  4. Na página **Configurações de Proteção,** configure as seguintes configurações:
     - Ativar **Selecione a ação para URLs potencialmente mal-intencionadas desconhecidas em mensagens**.
     - Selecione **Aplicar links seguros a mensagens enviadas dentro da organização**.

  Para obter mais informações, [consulte Set up Cofre Links policies in Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
