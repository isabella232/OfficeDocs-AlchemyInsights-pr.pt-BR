---
title: Sincronização de UPN desabilitada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726092"
---
# <a name="upn-sync-disabled"></a>Sincronização de UPN desabilitada

Se você iniciou a sincronização para o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do Azure AD PowerShell para habilitar a correspondência de UPN para a sua organização somente:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
A correspondência de disco UPN é automaticamente ativada para organizações que iniciaram a sincronização para o Azure AD no ou após 30 de março de 2016.
  
Para saber mais sobre a habilitação de correspondências por UPN e outros recursos de sincronização, confira [recursos do serviço de sincronização do Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

