---
title: Usar a opção de desbloqueio de impressão digital no Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796665"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="5d91d-102">Usar a opção de desbloqueio de impressão digital no Windows 10</span><span class="sxs-lookup"><span data-stu-id="5d91d-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="5d91d-103">**Habilitar impressão digital do Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="5d91d-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="5d91d-104">Para desbloquear o Windows 10 usando sua impressão digital, você precisa configurar a Impressão Digital do Windows Hello adicionando (deixando o Windows aprender a reconhecer) pelo menos um dedo.</span><span class="sxs-lookup"><span data-stu-id="5d91d-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="5d91d-105">Vá para **Configurações > Contas > opções de** login (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="5d91d-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5d91d-106">As opções de login disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="5d91d-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="5d91d-107">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="5d91d-107">For example:</span></span>

    ![Opções de login.](media/sign-in-options.png)

2. <span data-ttu-id="5d91d-109">Clique ou toque em **Impressão Digital do Windows Hello** e clique em **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="5d91d-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="5d91d-110">Na janela de configuração do Windows Hello, clique **em Iniciar**.</span><span class="sxs-lookup"><span data-stu-id="5d91d-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="5d91d-111">O sensor de impressão digital será ativado e você será solicitado a colocar o dedo no sensor:</span><span class="sxs-lookup"><span data-stu-id="5d91d-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor de impressão digital.](media/fingerprint-sensor.png)

3. <span data-ttu-id="5d91d-113">Siga as instruções, que solicitarão que você digitalizar repetidamente o dedo.</span><span class="sxs-lookup"><span data-stu-id="5d91d-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="5d91d-114">Quando isso for concluído, você terá a opção de adicionar outros dedos que talvez queira usar para entrar.</span><span class="sxs-lookup"><span data-stu-id="5d91d-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="5d91d-115">Na próxima vez que entrar no Windows 10, você terá a opção de usar sua impressão digital para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="5d91d-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="5d91d-116">**Impressão digital do Windows Hello não está disponível como uma opção de login**</span><span class="sxs-lookup"><span data-stu-id="5d91d-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="5d91d-117">Se a Impressão Digital do Windows Hello não for mostrada como uma opção nas opções de **Login,** isso significa que o Windows não está ciente de nenhum leitor/scanner de impressão digital anexado ao computador ou que uma política do sistema impede seu uso (se, por exemplo, seu computador for gerenciado pelo seu local de trabalho).</span><span class="sxs-lookup"><span data-stu-id="5d91d-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="5d91d-118">Para solucionar problemas:</span><span class="sxs-lookup"><span data-stu-id="5d91d-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="5d91d-119">Selecione o **botão Iniciar** na Barra de Tarefas e procure o Gerenciador **de Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="5d91d-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="5d91d-120">Clique ou toque para abrir **o Gerenciador de Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="5d91d-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="5d91d-121">No Gerenciador de Dispositivos, expanda dispositivos biométricos clicando em seu chevron.</span><span class="sxs-lookup"><span data-stu-id="5d91d-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. <span data-ttu-id="5d91d-123">Seu scanner de impressão digital deve ser listado como um dispositivo biométrico, como o scanner WBDI Synaptics:</span><span class="sxs-lookup"><span data-stu-id="5d91d-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="5d91d-125">Se o scanner de impressão digital não for mostrado e o scanner estiver integrado ao computador, vá para o site do fabricante do computador.</span><span class="sxs-lookup"><span data-stu-id="5d91d-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="5d91d-126">Na seção suporte técnico para seu modelo de computador, procure um driver do Windows 10 para um scanner que você pode instalar.</span><span class="sxs-lookup"><span data-stu-id="5d91d-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="5d91d-127">Se o scanner estiver separado do computador (anexado via USB), vá para o site do fabricante do scanner para encontrar e instalar o software de driver de dispositivo do Windows 10 para o modelo de scanner que você tem.</span><span class="sxs-lookup"><span data-stu-id="5d91d-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
