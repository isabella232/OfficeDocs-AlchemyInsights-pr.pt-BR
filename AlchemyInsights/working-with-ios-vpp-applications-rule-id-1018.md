---
title: Trabalhando com iOS VPP 1018 de Id de regra de aplicativos
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275276"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="0964f-102">Trabalhando com iOS VPP aplicativos</span><span class="sxs-lookup"><span data-stu-id="0964f-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="0964f-103">Leia [como gerenciar aplicativos de iOS adquiridos por meio de um programa de compra do volume com Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para fazer uso do programa de compra de Volume da Apple e o suporte para ele no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0964f-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="0964f-104">**Problemas comuns:** "Eu atribuída a um aplicativo VPP iOS a meus usuários, mas a instalação falhou."</span><span class="sxs-lookup"><span data-stu-id="0964f-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="0964f-p101">Isso pode acontecer se um único token VPP for usado em vários provedores de gerenciamento de dispositivo móvel. Tokens VPP da Apple só podem ser usados com um provedor. Se você tiver usado um token VPP com vários provedores, você deve reenvie o token para Intune.</span><span class="sxs-lookup"><span data-stu-id="0964f-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="0964f-p102">A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para exibir um relatório de uso de suas licenças, vá para o **Intune Mobile apps** \> página **licenças de aplicativo** . Para saber como recuperar licenças em uso, consulte [neste artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="0964f-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

