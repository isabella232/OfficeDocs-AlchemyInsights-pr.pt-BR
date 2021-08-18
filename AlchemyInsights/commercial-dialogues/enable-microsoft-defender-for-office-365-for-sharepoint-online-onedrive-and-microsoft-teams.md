---
title: Habilitar Cofre anexos para SharePoint Online, OneDrive e Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332367"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar Cofre anexos para SharePoint Online, OneDrive e Microsoft Teams

1. Usando suas credenciais de administrador global ou administrador de segurança, abra o portal Microsoft 365 Defender em e, em seguida, vá para Políticas & regras Políticas de ameaça <https://security.microsoft.com>  \>  \> **Cofre Anexos** na **seção Políticas**

   Para ir diretamente para a página **Cofre Anexos,** use <https://security.microsoft.com/safeattachmentv2> .

2. Na página **Cofre Anexos,** clique em **Configurações globais**.
3. No sobrevoo exibido, selecione Ativar o Microsoft Defender para Office 365 para **SharePoint, OneDrive** e Microsoft Teams e, em seguida, selecione **Salvar**.

    **Dica:** Faça as seguintes etapas para aprimorar a proteção de Cofre anexos para SharePoint, OneDrive e Microsoft Teams:
    - Para impedir que os usuários baixem arquivos mal-intencionados, use o valor do parâmetro `$true` *DisallowInfectedFileDownload* no cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** no SharePoint PowerShell Online. Para obter mais informações, consulte Use SharePoint Online PowerShell para impedir que os usuários [baixem arquivos mal-intencionados.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Criar uma política de alerta para arquivos detectados](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Para obter mais informações, [consulte Cofre Attachments for Office 365 for SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
