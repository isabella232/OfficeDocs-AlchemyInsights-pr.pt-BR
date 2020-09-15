---
title: ATP para SharePoint, OneDrive e Microsoft Teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715549"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP para SharePoint, OneDrive e Microsoft Teams

Siga estas etapas para habilitar a proteção avançada contra ameaças:

1. Acesse [https://protection.office.com](https://protection.office.com) e entre com uma conta de administrador global ou administrador de segurança.

2. No painel de navegação esquerdo em **Gerenciamento de ameaças**, **Policy** escolha \> **anexos seguros**da política.

3. Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams**.

4. [Crie uma política de alerta de atividade](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para receber notificações quando detectarmos arquivos mal-intencionados.

Para obter instruções completas, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Observação**: por design, a ATP não examina todos os arquivos no SharePoint Online, no onedrive for Business ou no Microsoft Teams. Os arquivos são verificados de forma assíncrona por um processo que usa atividade de compartilhamento, atividade de convidado e sinais de ameaça para identificar arquivos mal-intencionados. Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
