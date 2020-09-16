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
# <a name="upn-sync-disabled"></a><span data-ttu-id="1b720-102">Sincronização de UPN desabilitada</span><span class="sxs-lookup"><span data-stu-id="1b720-102">UPN sync disabled</span></span>

<span data-ttu-id="1b720-103">Se você iniciou a sincronização para o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do Azure AD PowerShell para habilitar a correspondência de UPN para a sua organização somente:</span><span class="sxs-lookup"><span data-stu-id="1b720-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="1b720-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="1b720-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="1b720-105">A correspondência de disco UPN é automaticamente ativada para organizações que iniciaram a sincronização para o Azure AD no ou após 30 de março de 2016.</span><span class="sxs-lookup"><span data-stu-id="1b720-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="1b720-106">Para saber mais sobre a habilitação de correspondências por UPN e outros recursos de sincronização, confira [recursos do serviço de sincronização do Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="1b720-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

