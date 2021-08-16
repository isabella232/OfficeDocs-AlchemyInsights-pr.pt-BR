---
title: Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058854"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams

1. Usando suas credenciais de administrador global ou de administrador de segurança, faça logoff no Centro de Conformidade e Segurança [Office 365 segurança.](https://protection.office.com/)
2. Selecione **Gerenciamento de ameaças** no painel esquerdo e selecione **Política**  >  [Cofre anexos](https://protection.office.com/safeattachment).
3. Selecione **Ativar o Microsoft Defender para Office 365 para SharePoint, OneDrive** e Microsoft Teams e, em seguida, selecione **Salvar**.
    > [!TIP]
    >
    > - Como administrador global ou administrador SharePoint Online, execute o seguinte cmdlet do PowerShell com o parâmetro **DisallowInfectedFileDownload** definido como *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurar alertas para arquivos detectados](https://go.microsoft.com/fwlink/?linkid=2092110)

Para obter mais informações, consulte [Microsoft Defender for Office 365 for SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
