---
title: Modifique o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897365"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="4261c-102">Modifique o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados</span><span class="sxs-lookup"><span data-stu-id="4261c-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="4261c-103">Por exemplo, no Windows, para armazenar os dados do perfil sob os dados do aplicativo local do usuário, em vez de no local padrão, configure a política *UserDataDir* para **${local_app_data}\Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="4261c-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="4261c-104">Para saber mais, consulte [Criar variáveis de diretório de dados do usuário do Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span><span class="sxs-lookup"><span data-stu-id="4261c-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>