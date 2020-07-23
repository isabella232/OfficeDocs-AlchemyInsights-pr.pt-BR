---
title: Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186089"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="3a0b3-102">Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a0b3-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="3a0b3-103">Se, durante a sincronização, você receber erros como “Um objeto sincronizado com o mesmo ProxyAddress ou UserPrincipalName já existe no seu diretório, confira o artigo [Diagnosticar e corrigir erros de sincronização relativos a atributos duplicados](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="3a0b3-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="3a0b3-104">Além disso, pense em ativar a resiliência de atributos duplicados.</span><span class="sxs-lookup"><span data-stu-id="3a0b3-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="3a0b3-105">Para saber mais, confira o artigo [Sincronização de identidade e resiliência de atributos duplicados](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="3a0b3-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>