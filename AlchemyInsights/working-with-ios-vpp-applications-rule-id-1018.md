---
title: Trabalhando com o ID de regra de aplicativos VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688934"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="5df39-102">Trabalhar com aplicativos VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="5df39-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="5df39-103">Leia [como gerenciar aplicativos Ios adquiridos por meio de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para usar o Apple Volume Purchase Program e o suporte para ele no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5df39-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="5df39-104">**Problemas comuns:** "Atribuí um aplicativo VPP iOS a meus usuários, mas a instalação falhou."</span><span class="sxs-lookup"><span data-stu-id="5df39-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="5df39-105">Isso pode acontecer quando um único token VPP é usado em vários provedores de gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="5df39-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="5df39-106">Os tokens de VPP da Apple só podem ser usados com um provedor.</span><span class="sxs-lookup"><span data-stu-id="5df39-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="5df39-107">Se você usou um token VPP com vários provedores, você deve recarregar o token para o Intune.</span><span class="sxs-lookup"><span data-stu-id="5df39-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="5df39-108">A instalação também pode falhar se o número total de instalações exceder o número de licenças.</span><span class="sxs-lookup"><span data-stu-id="5df39-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="5df39-109">Para exibir um relatório de uso para suas licenças, acesse a página licenças de aplicativos **móveis do Intune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="5df39-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="5df39-110">Para saber como recuperar licenças em uso, consulte [Este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="5df39-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
