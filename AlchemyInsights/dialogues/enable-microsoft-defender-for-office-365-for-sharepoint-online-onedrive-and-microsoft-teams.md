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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552247"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams

1. Usando suas credenciais de administrador global ou administrador de segurança, faça logoff no Centro de Conformidade e Segurança do [Office 365.](https://protection.office.com/)
2. Selecione **Gerenciamento de ameaças** no painel esquerdo e selecione **Anexos seguros** de  >  [política.](https://protection.office.com/safeattachment)
3. Selecione **Ativar o Microsoft Defender para Office 365 para SharePoint, OneDrive** e Microsoft Teams e selecione **Salvar**.
    > [!TIP]
    >
    > - Como administrador global ou administrador do SharePoint Online, execute o seguinte cmdlet do PowerShell com o parâmetro **DisallowInfectedFileDownload** definido como *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurar alertas para arquivos detectados](https://go.microsoft.com/fwlink/?linkid=2092110)

Para obter mais informações, consulte [Microsoft Defender for Office 365 for SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
