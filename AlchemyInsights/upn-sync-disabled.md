---
title: Sincronização UPN desabilitada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038100"
---
# <a name="upn-sync-disabled"></a>Sincronização UPN desabilitada

Se você começou a sincronizar com o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do Azure AD PowerShell para habilitar apenas a habilitação de match suave UPN para sua organização:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
A suspensão de UPN é automaticamente ativado para organizações que começaram a sincronizar com o Azure AD em ou após 30 de março de 2016.
  
Para saber mais sobre a habilitação de uma combinação suave em UPN e outros recursos de sincronização, consulte [Azure AD Conexão de serviço de sincronização.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

