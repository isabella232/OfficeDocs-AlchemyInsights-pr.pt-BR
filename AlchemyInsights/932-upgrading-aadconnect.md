---
title: 932 AADConnect atualizando
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937932"
---
# <a name="upgrade-azure-ad-connect"></a>Conecte-se a atualização Azure AD.

Por padrão, a atualização automática está habilitada para conectar Azure do AD, que ajuda a garantir que você está executando a versão mais recente. Para verificar as configurações de atualização automáticas, use o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell do Windows Azure AD. O cmdlet retornará um dos seguintes valores: 
  
- **Habilitado**: atualização automática está habilitada. 
    
- **Desabilitado**: atualização automática está desativada. 
    
- **Suspended**: O sistema não está mais elegível para receber atualizações automáticas. Você só poderá definir esse valor; ela é definida pelo sistema. 
    
Para obter mais informações, consulte [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Para baixar a versão mais recente do Connect do Azure AD, vá para [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

