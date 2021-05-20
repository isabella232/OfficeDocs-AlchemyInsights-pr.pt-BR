---
title: Habilitar Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543916"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams

1. Acesse https://protection.office.com e entre.
2. Escolha **Política de Gerenciamento** de Ameaças Cofre  >    >  **Anexos**.
3. Selecione **Ativar o Defender para Office 365 para SharePoint, OneDrive** e Microsoft Teams e clique em **Salvar**.
4. (Recomendado) Como administrador global ou administrador SharePoint Online, execute o cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true*.
5. (Recomendado) [Configurar alertas para](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) arquivos detectados.

> [!NOTE]
> O Microsoft Defender para Office 365 não examinará todos os arquivos no SharePoint Online, OneDrive ou Microsoft Teams. Os arquivos são verificados de forma assíncrona, por meio de um processo que usa eventos de compartilhamento e atividades de convidados, juntamente com heurísticas inteligentes e sinais de ameaça para identificar arquivos mal-intencionados. Consulte [Microsoft Defender for Office 365 for SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).