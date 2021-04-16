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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782139"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="6fb2c-102">Sincronização UPN desabilitada</span><span class="sxs-lookup"><span data-stu-id="6fb2c-102">UPN sync disabled</span></span>

<span data-ttu-id="6fb2c-103">Se você começou a sincronizar com o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do Azure AD PowerShell para habilitar apenas a habilitação de match suave UPN para sua organização:</span><span class="sxs-lookup"><span data-stu-id="6fb2c-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="6fb2c-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="6fb2c-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="6fb2c-105">A suspensão de UPN é automaticamente ativado para organizações que começaram a sincronizar com o Azure AD em ou após 30 de março de 2016.</span><span class="sxs-lookup"><span data-stu-id="6fb2c-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="6fb2c-106">Para saber mais sobre a habilitação de uma combinação suave em UPN e outros recursos de sincronização, consulte Recursos de serviço de sincronização [do Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="6fb2c-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

