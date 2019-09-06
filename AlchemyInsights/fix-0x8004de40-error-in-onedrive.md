---
title: Corrigir o erro 0x8004de40 no OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755836"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="24b3f-102">Corrigir o erro 0x8004de40 no OneDrive</span><span class="sxs-lookup"><span data-stu-id="24b3f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="24b3f-103">Se você receber um erro 0x8004de40 com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="24b3f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="24b3f-104">Reinicie o computador afetado enquanto estiver conectado ao seu domínio de diretório do acitve.</span><span class="sxs-lookup"><span data-stu-id="24b3f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="24b3f-105">Se uma reinicialização não corrigir o problema, desingresse e reingresse seu dispositivo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24b3f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="24b3f-106">**Observação**: você deve estar em sua rede corporativa enquanto executa estas etapas.</span><span class="sxs-lookup"><span data-stu-id="24b3f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="24b3f-107">Não execute estas etapas quando não puder se conectar à infraestrutura corporativa (por exemplo, ao viajar).</span><span class="sxs-lookup"><span data-stu-id="24b3f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="24b3f-108">Abra um prompt de comando com privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="24b3f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="24b3f-109">Para abrir um prompt de comando com privilégios elevados, clique em **Iniciar**, clique com o botão direito do mouse em **prompt de comando**e clique em **Executar como administrador**.</span><span class="sxs-lookup"><span data-stu-id="24b3f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="24b3f-110">Digite *dsregcmd/Leave* e pressione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="24b3f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="24b3f-111">Ao concluir, digite *dsregcmd/Join* e pressione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="24b3f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="24b3f-112">Ao concluir, feche o prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="24b3f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="24b3f-113">Reinicie o computador e faça logon no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="24b3f-113">Reboot the computer, and log into OneDrive.</span></span>