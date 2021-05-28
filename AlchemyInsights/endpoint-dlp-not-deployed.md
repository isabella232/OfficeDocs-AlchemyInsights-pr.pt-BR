---
title: O Ponto de extremidade da DLP não foi implantado no dispositivo do usuário
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694799"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="769d2-102">O Ponto de extremidade da DLP não foi implantado no dispositivo do usuário</span><span class="sxs-lookup"><span data-stu-id="769d2-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="769d2-103">Se a configuração da Prevenção contra perda de dados de Ponto de Extremidade (DLP) do ponto de extremidade não foi aplicada ao dispositivo de um usuário, confirme se você atende a estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="769d2-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="769d2-104">O Windows 10 x64 build 1809 ou posterior está instalado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="769d2-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="769d2-105">O cliente anti-malware versão 4.18.2009.7 ou posterior está instalado.</span><span class="sxs-lookup"><span data-stu-id="769d2-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="769d2-106">O dispositivo é **um** destes:</span><span class="sxs-lookup"><span data-stu-id="769d2-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="769d2-107">Azure Active Directory (Azure AD) ingressou</span><span class="sxs-lookup"><span data-stu-id="769d2-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="769d2-108">Ingressado no Azure AD híbrido</span><span class="sxs-lookup"><span data-stu-id="769d2-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="769d2-109">AAD registrado</span><span class="sxs-lookup"><span data-stu-id="769d2-109">AAD registered</span></span>

- <span data-ttu-id="769d2-110">Para impor ações de política, certifique-se de que o navegador Microsoft Chromium Edge esteja instalado no dispositivo do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="769d2-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="769d2-111">Para requisitos adicionais para implantação do Ponto de extremidade da DLP, confira [Primeiros passos com a Prevenção contra perda de dados de Ponto de Extremidade](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="769d2-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>