---
title: Sincronização UPN desabilitada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921696"
---
# <a name="upn-sync-disabled"></a>Sincronização UPN desabilitada

Se você tiver iniciado a sincronização do Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do PowerShell do Windows Azure AD para habilitar a correspondência suave UPN para a sua organização somente:
  
 **Set-MsolDirSyncFeature-EnableSoftMatchOnUpn de recurso-habilitar $True**
  
Correspondência UPN suave é ativada automaticamente para organizações que iniciou a sincronização do Azure AD em ou após 30 de março de 2016.
  
Para saber mais sobre como habilitar a correspondência suave em UPN e outros recursos de sincronização, consulte [recursos do serviço de sincronização de conectar do Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

