---
title: Microsoft Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: c42786559d527a5ef9a0a8cfad1476f4d122b6d5570ca5b9ea138b21a153ae96
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896323"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams

Siga estas etapas para habilitar o Microsoft Defender para Office 365:

1. Acesse e [https://protection.office.com](https://protection.office.com) entre com uma conta de administrador global ou administrador de segurança.

2. No painel de navegação esquerdo em **Gerenciamento de ameaças,** escolha **Política** \> **Cofre Anexos**.

3. Selecione **Ativar o Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams**.

4. [Crie uma política de alerta de atividade](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para receber notificações quando detectarmos arquivos mal-intencionados.

Para obter instruções [completas,](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)consulte o guia Ativar Cofre anexos para SharePoint, OneDrive e Microsoft Teams .

**Observação**: por design, o Microsoft Defender para Office 365 não digitalizar todos os arquivos no SharePoint Online, OneDrive for Business ou Microsoft Teams. Os arquivos são verificados de forma assíncrona por um processo que usa sinais de atividade de compartilhamento, atividade de convidado e ameaças para identificar arquivos mal-intencionados. Para obter mais informações, [consulte Cofre Attachments for SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
