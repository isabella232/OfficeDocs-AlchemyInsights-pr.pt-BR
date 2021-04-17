---
title: Configurações de inicialização no Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828140"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="b00af-102">Configurações de inicialização no Windows 10</span><span class="sxs-lookup"><span data-stu-id="b00af-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="b00af-103">**Alterar quais aplicativos são executados automaticamente na inicialização**</span><span class="sxs-lookup"><span data-stu-id="b00af-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="b00af-104">Vá para [Configurações > Aplicativos > Inicialização](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="b00af-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="b00af-105">Certifique-se de que qualquer aplicativo que você deseja executar na inicialização está **ligado**.</span><span class="sxs-lookup"><span data-stu-id="b00af-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="b00af-106">**Adicionar um aplicativo para ser executado automaticamente na inicialização**</span><span class="sxs-lookup"><span data-stu-id="b00af-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="b00af-107">Clique ou toque **em Iniciar** e encontre o aplicativo que você deseja executar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="b00af-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="b00af-108">Clique com o botão direito do mouse no aplicativo, clique em **Mais** e clique **em Abrir local do arquivo**.</span><span class="sxs-lookup"><span data-stu-id="b00af-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="b00af-109">Isso abre o local onde o atalho para o aplicativo é salvo.</span><span class="sxs-lookup"><span data-stu-id="b00af-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="b00af-110">Se não houver opção para o local do arquivo Open, isso significa que o aplicativo não pode ser executado na inicialização.</span><span class="sxs-lookup"><span data-stu-id="b00af-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="b00af-111">Com o local do arquivo aberto, pressione a tecla **de logotipo do Windows + R**, digite **shell:inicialização,** clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="b00af-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="b00af-112">Isso abre a pasta Inicialização.</span><span class="sxs-lookup"><span data-stu-id="b00af-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="b00af-113">Copie e colar o atalho para o aplicativo do local do arquivo para a pasta Inicialização.</span><span class="sxs-lookup"><span data-stu-id="b00af-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="b00af-114">**Opções de inicialização avançadas (incluindo Modo de Segurança, configurações UEFI e inicialização de outro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="b00af-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="b00af-115">Salve seu trabalho e feche todos os documentos abertos, pois essas etapas reiniciarão o computador.</span><span class="sxs-lookup"><span data-stu-id="b00af-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="b00af-116">Vá para [Configurações > Atualização & Segurança > Recuperação](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="b00af-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="b00af-117">Em **Inicialização avançada,** clique **em Reiniciar agora**.</span><span class="sxs-lookup"><span data-stu-id="b00af-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="b00af-118">Depois que o computador é reiniciado para a tela Escolher uma opção:</span><span class="sxs-lookup"><span data-stu-id="b00af-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="b00af-119">Para inicializar de um dispositivo como uma unidade USB, clique **em Usar um dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="b00af-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="b00af-120">Para inserir as configurações uefi (às vezes chamada de configuração do BIOS), clique em Solucionar problemas > **opções avançadas > Configurações de Firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="b00af-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="b00af-121">Para inserir o Modo de Segurança ou alterar as configurações de inicialização avançadas, clique em **Solucionar problemas > opções avançadas**> Configurações de Inicialização, em seguida, clique em **Reiniciar**.</span><span class="sxs-lookup"><span data-stu-id="b00af-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="b00af-122">Você pode ser solicitado a inserir sua chave de [recuperação do BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="b00af-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="b00af-123">Depois que o computador reiniciar novamente, clique na configuração de inicialização que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="b00af-123">After your PC restarts again, click the startup setting you want to use.</span></span>