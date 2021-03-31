---
title: Definir o Microsoft Edge como navegador padrão em um dispositivo macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426757"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="5df07-102">Definir o Microsoft Edge como navegador padrão em um dispositivo macOS</span><span class="sxs-lookup"><span data-stu-id="5df07-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="5df07-103">Use um desses dois métodos para definir o Microsoft Edge como navegador padrão:</span><span class="sxs-lookup"><span data-stu-id="5df07-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="5df07-104">Método 1: Atualize o dispositivo com uma imagem do macOS onde o Microsoft Edge já foi configurado como navegador padrão.</span><span class="sxs-lookup"><span data-stu-id="5df07-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="5df07-105">Método 2: Defina a política DefaultBrowserSettingEnabled para solicitar ao usuário que defina o Microsoft Edge como navegador padrão.</span><span class="sxs-lookup"><span data-stu-id="5df07-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="5df07-106">Qualquer um dos métodos permite que o usuário altere o navegador padrão.</span><span class="sxs-lookup"><span data-stu-id="5df07-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="5df07-107">Por esse motivo, recomendamos que você implante a política DefaultBrowserSettingEnabled mesmo se tiver usado o método 1.</span><span class="sxs-lookup"><span data-stu-id="5df07-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="5df07-108">Se um usuário alterar o navegador padrão depois que a política for implantada, a política solicitará que o usuário defina o navegador padrão de volta para o Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5df07-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
