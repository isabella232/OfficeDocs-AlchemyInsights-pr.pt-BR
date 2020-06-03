---
title: Habilitar o Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506906"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar a proteção avançada contra ameaças do Office 365 para o SharePoint Online, o OneDrive e o Microsoft Teams

1. Acesse https://protection.office.com e entre.
2. Escolha **Threat management**  >  **Policy**  >  **anexos seguros**da política de gerenciamento de ameaças.
3. Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams**e clique em **salvar**.
4. Recomenda Como administrador global ou administrador do SharePoint Online, execute o cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true*.
5. Recomenda [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para arquivos detectados.

> [!NOTE]
> A ATP deixará a verificação de todos os arquivos no SharePoint Online, no OneDrive ou no Microsoft Teams. Os arquivos são verificados de forma assíncrona por meio de um processo que usa eventos de atividade de compartilhamento e convidados, juntamente com heurística inteligente e sinais de ameaça para identificar arquivos mal-intencionados. Consulte [ATP para SharePoint, onedrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).