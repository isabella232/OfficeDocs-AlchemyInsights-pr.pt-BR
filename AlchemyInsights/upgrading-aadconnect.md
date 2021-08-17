---
title: 932 Atualizando o AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104800"
---
# <a name="upgrade-azure-ad-connect"></a>Atualizar o Azure AD Conexão

Por padrão, a atualização automática está habilitada para o Azure AD Conexão, o que ajuda a garantir que você esteja executando a versão mais recente. Para verificar as configurações de atualização automáticas, use o cmdlet **Get-ADSyncAutoUpgrade** no Azure AD PowerShell. O cmdlet retornará um dos seguintes valores:

- **Habilitado :** A atualização automática está habilitada.

- **Desabilitado**: a atualização automática está desabilitada.

- **Suspenso**: o sistema não está mais qualificado para receber atualizações automáticas. Você não pode configurar esse valor; ele é definido pelo sistema.

Para obter mais informações, consulte [Atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Para baixar a versão mais recente do Azure AD Conexão, acesse [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
