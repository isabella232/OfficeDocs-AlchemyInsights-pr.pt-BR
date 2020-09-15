---
title: Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713442"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="f63a8-102">Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f63a8-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="f63a8-103">Se, durante a sincronização, você receber erros como “Um objeto sincronizado com o mesmo ProxyAddress ou UserPrincipalName já existe no seu diretório, confira o artigo [Diagnosticar e corrigir erros de sincronização relativos a atributos duplicados](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="f63a8-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="f63a8-104">Além disso, pense em ativar a resiliência de atributos duplicados.</span><span class="sxs-lookup"><span data-stu-id="f63a8-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="f63a8-105">Para saber mais, confira o artigo [Sincronização de identidade e resiliência de atributos duplicados](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="f63a8-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>