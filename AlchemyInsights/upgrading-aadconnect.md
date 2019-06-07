---
title: 932 atualizando AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757279"
---
# <a name="upgrade-azure-ad-connect"></a>Atualizar Azure AD Connect

Por padrão, a atualização automática está habilitada para o Azure AD Connect, o que ajuda a garantir que você esteja executando a versão mais recente. Para verificar as configurações de atualização automática, use o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell do Azure AD. O cmdlet retornará um dos seguintes valores: 

- **Habilitado**: a atualização automática está habilitada.

- **Disabled**: a atualização automática está desabilitada.

- **Suspenso**: o sistema não está mais qualificado para receber atualizações automáticas. Você não pode configurar esse valor; é definido pelo sistema. 

Para obter mais informações, consulte [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Para baixar a versão mais recente do Azure AD Connect, acesse [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
