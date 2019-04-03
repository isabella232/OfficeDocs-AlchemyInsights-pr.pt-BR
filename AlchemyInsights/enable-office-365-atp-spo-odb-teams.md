---
title: Habilitar o Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030878"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar a proteção avançada contra ameaças do Office 365 para o SharePoint Online, o OneDrive e o Microsoft Teams

1. Acesse https://protection.office.com e entre.
2. Escolha**anexos seguros**da**política** > de **Gerenciamento** > de ameaças.
3. Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams**e clique em **salvar**.
4. Recomenda Como administrador global ou administrador do SharePoint Online, execute o cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true*.
5. Recomenda [Configurar alertas](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para arquivos detectados.

> [!NOTE]
> A ATP deixará a verificação de todos os arquivos no SharePoint Online, no OneDrive ou no Microsoft Teams. Os arquivos são verificados de forma assíncrona por meio de um processo que usa eventos de atividade de compartilhamento e convidados, juntamente com heurística inteligente e sinais de ameaça para identificar arquivos mal-intencionados. Ver [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).