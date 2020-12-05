---
title: Suporte da Microsoft para o Microsoft defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576355"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="41d61-102">Suporte da Microsoft para o Microsoft defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="41d61-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="41d61-103">Projetado para o Windows 10 e o Microsoft Edge, o Application Guard usa uma abordagem de isolamento de hardware que permite que um usuário navegue em um site não confiável de dentro de um contêiner isolado, Hyper-V –, separado do sistema operacional host.</span><span class="sxs-lookup"><span data-stu-id="41d61-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="41d61-104">Um administrador corporativo define uma lista de sites confiáveis, recursos de nuvem e redes internas.</span><span class="sxs-lookup"><span data-stu-id="41d61-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="41d61-105">Quando um usuário visita um site que não está na lista, o Microsoft Edge abrirá o site no contêiner.</span><span class="sxs-lookup"><span data-stu-id="41d61-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="41d61-106">Isso significa que, se o site for mal-intencionado, o computador host permanecerá protegido e o invasor não receberá os dados da empresa.</span><span class="sxs-lookup"><span data-stu-id="41d61-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="41d61-107">A instalação de extensões no contêiner tem suporte da versão 81 do Microsoft Edge e pode ser controlada por uma política.</span><span class="sxs-lookup"><span data-stu-id="41d61-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="41d61-108">O endereço updateURL que é usado na política ExtensionInstallForcelist deve ser adicionado como um recurso neutro nas diretivas de isolamento de rede usadas pelo Application Guard.</span><span class="sxs-lookup"><span data-stu-id="41d61-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="41d61-109">Para obter mais informações, consulte [suporte do Microsoft Edge para o Microsoft defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="41d61-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
