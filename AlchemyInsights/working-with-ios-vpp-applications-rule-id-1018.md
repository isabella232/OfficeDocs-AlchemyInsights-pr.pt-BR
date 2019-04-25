---
title: Trabalhando com o ID de regra de aplicativos VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420472"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="8238b-102">Trabalhar com aplicativos VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="8238b-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="8238b-103">Leia [como gerenciar aplicativos Ios adquiridos por meio de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para usar o Apple Volume Purchase Program e o suporte para ele no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8238b-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="8238b-104">**Problemas comuns:** "Atribuí um aplicativo VPP iOS a meus usuários, mas a instalação falhou."</span><span class="sxs-lookup"><span data-stu-id="8238b-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="8238b-105">Isso pode acontecer quando um único token VPP é usado em vários provedores de gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="8238b-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="8238b-106">Os tokens de VPP da Apple só podem ser usados com um provedor.</span><span class="sxs-lookup"><span data-stu-id="8238b-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="8238b-107">Se você usou um token VPP com vários provedores, você deve recarregar o token para o Intune.</span><span class="sxs-lookup"><span data-stu-id="8238b-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="8238b-108">A instalação também pode falhar se o número total de instalações exceder o número de licenças.</span><span class="sxs-lookup"><span data-stu-id="8238b-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="8238b-109">Para exibir um relatório de uso para suas licenças, acesse a página **licenças** de aplicativos **móveis** \> do Intune.</span><span class="sxs-lookup"><span data-stu-id="8238b-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="8238b-110">Para saber como recuperar licenças em uso, consulte [Este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="8238b-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

