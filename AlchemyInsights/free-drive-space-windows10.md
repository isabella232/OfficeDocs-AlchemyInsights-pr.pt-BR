---
title: Liberar espaço em disco no Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505344"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="141b6-102">Liberar espaço em disco no Windows 10</span><span class="sxs-lookup"><span data-stu-id="141b6-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="141b6-103">Veja duas opções para liberar espaço em disco no Windows:</span><span class="sxs-lookup"><span data-stu-id="141b6-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="141b6-104">Libere espaço em disco no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="141b6-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="141b6-105">Libere espaço para atualizações do Windows 10 com um dispositivo de armazenamento externo.</span><span class="sxs-lookup"><span data-stu-id="141b6-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="141b6-106">Se você ainda tiver pouco espaço em disco após usar a Limpeza de Disco, é possível que sua pasta Temp esteja enchendo rapidamente com arquivos de aplicativos (.appx) usados pela Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="141b6-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="141b6-107">Para resolver esse problema, redefina a Store, limpe o cache dela e, em seguida, execute a solução de problemas do Windows Update.</span><span class="sxs-lookup"><span data-stu-id="141b6-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="141b6-108">Verifique se a Microsoft Store está fechada antes de prosseguir com estas etapas.</span><span class="sxs-lookup"><span data-stu-id="141b6-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="141b6-109">**Etapa 1: Redefinir a Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="141b6-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="141b6-110">**Observação** Isso exclui permanentemente os dados do aplicativo no dispositivo, incluindo suas preferências e detalhes de entrada.</span><span class="sxs-lookup"><span data-stu-id="141b6-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="141b6-111">Selecione **Iniciar** > **Configurações** > **Aplicativos** > **Aplicativos e recursos**.</span><span class="sxs-lookup"><span data-stu-id="141b6-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="141b6-112">Na lista de aplicativos, localize e selecione a Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="141b6-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="141b6-113">Selecione **Opções avançadas**.</span><span class="sxs-lookup"><span data-stu-id="141b6-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="141b6-114">Role para baixo, selecione **Redefinir** e, em seguida **Confirmar Redefinição**.</span><span class="sxs-lookup"><span data-stu-id="141b6-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="141b6-115">**Etapa 2: Limpar o cache da Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="141b6-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="141b6-116">Pressione a Tecla do Logotipo do Windows + R para abrir a caixa de diálogo Executar.</span><span class="sxs-lookup"><span data-stu-id="141b6-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="141b6-117">Digite wsreset.exe e selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="141b6-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="141b6-118">Uma janela vazia do Prompt de Comando será aberta.</span><span class="sxs-lookup"><span data-stu-id="141b6-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="141b6-119">Após cerca de 10 segundos, a janela se fecha e a Store será aberta automaticamente.</span><span class="sxs-lookup"><span data-stu-id="141b6-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="141b6-120">**Etapa 3: Redefinir o Windows Update**</span><span class="sxs-lookup"><span data-stu-id="141b6-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="141b6-121">Selecione **Iniciar** > **Configurações** > **Atualização e Segurança** > **Solucionar problemas**.</span><span class="sxs-lookup"><span data-stu-id="141b6-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="141b6-122">Role para baixo, selecione **Windows Update** na lista e, em seguida, **Executar a solução de problemas**.</span><span class="sxs-lookup"><span data-stu-id="141b6-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="141b6-123">Reinicie o computador e verifique se você continua tendo problemas.</span><span class="sxs-lookup"><span data-stu-id="141b6-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

