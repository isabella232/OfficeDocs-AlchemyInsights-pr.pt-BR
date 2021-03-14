---
title: Remover o serviço de plano de fundo da Pesquisa da Microsoft no Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753378"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="d52bb-102">Remover o serviço de plano de fundo da Pesquisa da Microsoft no Bing</span><span class="sxs-lookup"><span data-stu-id="d52bb-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="d52bb-103">Para remover o serviço de segundo plano da Pesquisa da Microsoft no Bing, experimente as seguintes medidas:</span><span class="sxs-lookup"><span data-stu-id="d52bb-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="d52bb-104">Para reverter para as configurações originais do mecanismo de pesquisa, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d52bb-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="d52bb-105">a.</span><span class="sxs-lookup"><span data-stu-id="d52bb-105">a.</span></span> <span data-ttu-id="d52bb-106">Alterne o **Use o Bing como seu mecanismo de pesquisa padrão [para](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Desligado**.</span><span class="sxs-lookup"><span data-stu-id="d52bb-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="d52bb-107">b.</span><span class="sxs-lookup"><span data-stu-id="d52bb-107">b.</span></span> <span data-ttu-id="d52bb-108">[Vá para a Centro de administração do Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e limpe a configuração que afeta todos os usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d52bb-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="d52bb-109">Para remover o serviço de segundo plano de um dispositivo individual, faça as seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="d52bb-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="d52bb-110">a.</span><span class="sxs-lookup"><span data-stu-id="d52bb-110">a.</span></span> <span data-ttu-id="d52bb-111">Vá para **Painel de controle > Programas > Programas e Recursos**.</span><span class="sxs-lookup"><span data-stu-id="d52bb-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="d52bb-112">b.</span><span class="sxs-lookup"><span data-stu-id="d52bb-112">b.</span></span> <span data-ttu-id="d52bb-113">Clique com o botão direito em **Pesquisa da Microsoft no Bing** na lista de programas instalados e clique em **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="d52bb-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="d52bb-114">Para remover o serviço de segundo plano de vários dispositivos da sua organização, faça logon como administrador e execute o seguinte comando em um script:</span><span class="sxs-lookup"><span data-stu-id="d52bb-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
