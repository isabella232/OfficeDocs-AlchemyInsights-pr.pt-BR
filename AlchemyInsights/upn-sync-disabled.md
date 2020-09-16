---
title: Sincronização de UPN desabilitada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749502"
---
# <a name="upn-sync-disabled"></a>Sincronização de UPN desabilitada

Se você iniciou a sincronização para o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do Azure AD PowerShell para habilitar a correspondência de UPN para a sua organização somente:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
A correspondência de disco UPN é automaticamente ativada para organizações que iniciaram a sincronização para o Azure AD no ou após 30 de março de 2016.
  
Para saber mais sobre a habilitação de correspondências por UPN e outros recursos de sincronização, confira [recursos do serviço de sincronização do Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

