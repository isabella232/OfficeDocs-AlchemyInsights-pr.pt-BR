---
title: Usar Microsoft Intune para gerenciar o acesso à Web no Microsoft Edge para iOS e Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989642"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="d9b58-102">Usar Microsoft Intune para gerenciar o acesso à Web no Microsoft Edge para iOS e Android</span><span class="sxs-lookup"><span data-stu-id="d9b58-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="d9b58-103">Microsoft Edge para iOS e Android permite que um usuário navegue pela Web de vários perfis completamente separados.</span><span class="sxs-lookup"><span data-stu-id="d9b58-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="d9b58-104">Os recursos de proteção mais amplos para Microsoft 365 dados ficam disponíveis quando você se inscreve no pacote Enterprise Mobility + Security, que inclui recursos de Microsoft Intune e Azure Active Directory Premium, como acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="d9b58-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="d9b58-105">No mínimo, você vai querer implantar uma política de acesso condicional que (1) permite que os usuários se conectem de dispositivos móveis ao Microsoft Edge para iOS e Android e que (2) implemente uma política de proteção de aplicativos Microsoft Intune que fornece uma experiência de navegação protegida.</span><span class="sxs-lookup"><span data-stu-id="d9b58-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="d9b58-106">Para entender como você pode usar o acesso condicional e as políticas, consulte:</span><span class="sxs-lookup"><span data-stu-id="d9b58-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="d9b58-107">Aplicar Active Directory do Azure políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="d9b58-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="d9b58-108">Criar Microsoft Intune de proteção de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d9b58-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="d9b58-109">Usar o login único para Active Directory do Azure web conectados em navegadores protegidos por política</span><span class="sxs-lookup"><span data-stu-id="d9b58-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="d9b58-110">Usar a configuração do aplicativo para gerenciar a experiência de navegação</span><span class="sxs-lookup"><span data-stu-id="d9b58-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="d9b58-111">Permitir o uso de apenas contas de trabalho e de estudante</span><span class="sxs-lookup"><span data-stu-id="d9b58-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="d9b58-112">Implantar políticas gerais de configuração de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9b58-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="d9b58-113">Implantar políticas de configuração de aplicativos para proteção de dados</span><span class="sxs-lookup"><span data-stu-id="d9b58-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="d9b58-114">Usar Microsoft Endpoint Manager para implantar políticas de configuração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d9b58-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="d9b58-115">Para saber como acessar logs de aplicativos gerenciados, consulte Use Microsoft Edge para iOS e Android para acessar logs [de aplicativos gerenciados.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="d9b58-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
