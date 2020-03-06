---
title: Configurações de inicialização no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408907"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="d22f6-102">Configurações de inicialização no Windows 10</span><span class="sxs-lookup"><span data-stu-id="d22f6-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="d22f6-103">**Alterar quais aplicativos são executados automaticamente na inicialização**</span><span class="sxs-lookup"><span data-stu-id="d22f6-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="d22f6-104">Vá até [configurações > aplicativos > inicialização](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d22f6-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="d22f6-105">Certifique-se **de**que qualquer aplicativo que você deseja executar na inicialização esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="d22f6-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="d22f6-106">**Adicionar um aplicativo para ser executado automaticamente na inicialização**</span><span class="sxs-lookup"><span data-stu-id="d22f6-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="d22f6-107">Clique ou toque em **Iniciar** e localize o aplicativo que você deseja executar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="d22f6-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="d22f6-108">Clique com o botão direito do mouse no aplicativo, clique em **mais**e, em seguida, clique em **abrir local do arquivo**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="d22f6-109">Isso abre o local onde o atalho para o aplicativo é salvo.</span><span class="sxs-lookup"><span data-stu-id="d22f6-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="d22f6-110">Se não houver opção para abrir o local do arquivo, isso significa que o aplicativo não pode ser executado na inicialização.</span><span class="sxs-lookup"><span data-stu-id="d22f6-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="d22f6-111">Com o local do arquivo aberto, pressione a **tecla do logotipo do Windows + R**, digite **shell: Startup**e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="d22f6-112">Isso abre a pasta inicialização.</span><span class="sxs-lookup"><span data-stu-id="d22f6-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="d22f6-113">Copie e cole o atalho para o aplicativo do local do arquivo para a pasta de inicialização.</span><span class="sxs-lookup"><span data-stu-id="d22f6-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="d22f6-114">**Opções avançadas de inicialização (incluindo o modo de segurança, configurações de UEFI e inicialização a partir de outro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="d22f6-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="d22f6-115">Salve seu trabalho e feche todos os documentos abertos, pois essas etapas reiniciarão seu computador.</span><span class="sxs-lookup"><span data-stu-id="d22f6-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="d22f6-116">Vá até [configurações > atualização & segurança > recuperação](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d22f6-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="d22f6-117">Em **inicialização avançada**, clique em **reiniciar agora**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="d22f6-118">Após a reinicialização do computador para a tela escolha uma opção:</span><span class="sxs-lookup"><span data-stu-id="d22f6-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="d22f6-119">Para inicializar a partir de um dispositivo como uma unidade USB, clique em **usar um dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="d22f6-120">Para inserir as configurações de UEFI (às vezes chamadas de configuração de BIOS), clique em **solucionar problemas > opções avançadas > configurações de firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="d22f6-121">Para inserir o modo de segurança ou alterar as configurações de inicialização avançadas, clique em **solucionar problemas > opções avançadas > configurações de inicialização**e clique em **reiniciar**.</span><span class="sxs-lookup"><span data-stu-id="d22f6-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="d22f6-122">Você pode ser solicitado a inserir sua [chave de recuperação do BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="d22f6-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="d22f6-123">Após reiniciar o computador, clique na configuração de inicialização que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="d22f6-123">After your PC restarts again, click the startup setting you want to use.</span></span>