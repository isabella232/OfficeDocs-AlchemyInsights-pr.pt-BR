---
title: Solucionando problemas de monitor existente
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738557"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="c2115-102">Solucionar problemas de um monitor existente</span><span class="sxs-lookup"><span data-stu-id="c2115-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="c2115-103">Experimente estas soluções para solucionar problemas de um monitor.</span><span class="sxs-lookup"><span data-stu-id="c2115-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="c2115-104">**Atualize a exibição do seu monitor:**</span><span class="sxs-lookup"><span data-stu-id="c2115-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="c2115-105">Pressione as teclas a seguir ao mesmo tempo: tecla Windows + Ctrl + Shift + B. Isso atualizará a comunicação com seu driver de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c2115-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="c2115-106">Seus monitores piscarão momentaneamente e voltarão após alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="c2115-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="c2115-107">**Solucionar problemas de hardware do monitor:**</span><span class="sxs-lookup"><span data-stu-id="c2115-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="c2115-108">Desconecte o cabo que conecta o computador ao monitor e conecte-o novamente.</span><span class="sxs-lookup"><span data-stu-id="c2115-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="c2115-109">Desconecte qualquer dispositivo não essencial do seu computador (como adaptadores ou cais).</span><span class="sxs-lookup"><span data-stu-id="c2115-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="c2115-110">**Se você instalou recentemente uma atualização no computador, pode reverter o seu driver de vídeo:**</span><span class="sxs-lookup"><span data-stu-id="c2115-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="c2115-111">Selecione **Iniciar**, digite **Gerenciador de dispositivos**e selecione **Gerenciador de dispositivos** nos resultados.</span><span class="sxs-lookup"><span data-stu-id="c2115-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c2115-112">Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo, es selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="c2115-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="c2115-113">Navegue até a guia **Driver** e selecione **Reverter driver**.</span><span class="sxs-lookup"><span data-stu-id="c2115-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="c2115-114">Observação: se isso não estiver disponível ou estiver esmaecido, selecione **não** nas opções abaixo para mover para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="c2115-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="c2115-115">Talvez seja necessário reiniciar o computador para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="c2115-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="c2115-116">**Desinstalar e reinstalar o driver de vídeo:**</span><span class="sxs-lookup"><span data-stu-id="c2115-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="c2115-117">Selecione **Iniciar**, digite **Gerenciador de dispositivos**e selecione **Gerenciador de dispositivos** nos resultados.</span><span class="sxs-lookup"><span data-stu-id="c2115-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c2115-118">Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo, es selecione **desinstalar dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="c2115-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="c2115-119">Selecione a caixa ao lado de **excluir o software de driver para este dispositivo** e selecione **desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="c2115-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="c2115-120">Observação: você pode ser solicitado a reiniciar o computador neste estágio.</span><span class="sxs-lookup"><span data-stu-id="c2115-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="c2115-121">Certifique-se de anotar as instruções restantes antes de reiniciar.</span><span class="sxs-lookup"><span data-stu-id="c2115-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="c2115-122">Abra o Gerenciador de dispositivos novamente.</span><span class="sxs-lookup"><span data-stu-id="c2115-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="c2115-123">Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo e selecione **Atualizar driver**.</span><span class="sxs-lookup"><span data-stu-id="c2115-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="c2115-124">Selecione **Pesquisar automaticamente o software de driver de atualização** e siga as instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="c2115-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>