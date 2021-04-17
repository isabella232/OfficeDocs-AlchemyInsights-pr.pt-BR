---
title: Solução de problemas do monitor existente
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824567"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="d6cff-102">Solucionar problemas de um monitor existente</span><span class="sxs-lookup"><span data-stu-id="d6cff-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="d6cff-103">Experimente essas soluções para solucionar problemas de um monitor.</span><span class="sxs-lookup"><span data-stu-id="d6cff-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="d6cff-104">**Atualize a exibição do monitor:**</span><span class="sxs-lookup"><span data-stu-id="d6cff-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="d6cff-105">Pressione as seguintes teclas ao mesmo tempo: Windows Key + Ctrl + Shift + B. Isso atualizará a comunicação com o driver gráfico.</span><span class="sxs-lookup"><span data-stu-id="d6cff-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="d6cff-106">Seus monitores piscarão momentaneamente e voltarão depois de alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="d6cff-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="d6cff-107">**Solucionar problemas de hardware de monitoramento:**</span><span class="sxs-lookup"><span data-stu-id="d6cff-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="d6cff-108">Desconectar o cabo conectando seu computador ao monitor e conectá-lo novamente.</span><span class="sxs-lookup"><span data-stu-id="d6cff-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="d6cff-109">Desconecte os dispositivos não essenciais do computador (como adaptadores ou encaixes).</span><span class="sxs-lookup"><span data-stu-id="d6cff-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="d6cff-110">**Se você instalou recentemente uma atualização em seu computador, poderá reverter o driver de exibição:**</span><span class="sxs-lookup"><span data-stu-id="d6cff-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="d6cff-111">Selecione **Iniciar**, digite **gerenciador de dispositivos** e selecione Gerenciador de **Dispositivos** nos resultados.</span><span class="sxs-lookup"><span data-stu-id="d6cff-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d6cff-112">Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="d6cff-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="d6cff-113">Navegue até a guia **Driver** e selecione **Reverter Driver**.</span><span class="sxs-lookup"><span data-stu-id="d6cff-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="d6cff-114">Observação: se isso não estiver disponível ou estiver acinzado, selecione **Não** nas opções abaixo para mover para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="d6cff-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="d6cff-115">Talvez seja necessário reiniciar o computador antes que essas alterações entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="d6cff-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="d6cff-116">**Desinstalar e reinstalar o driver de exibição:**</span><span class="sxs-lookup"><span data-stu-id="d6cff-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="d6cff-117">Selecione **Iniciar**, digite **gerenciador de dispositivos** e selecione Gerenciador de **Dispositivos** nos resultados.</span><span class="sxs-lookup"><span data-stu-id="d6cff-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d6cff-118">Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione **Desinstalar o dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="d6cff-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="d6cff-119">Selecione a caixa ao lado de **Excluir o software de driver deste dispositivo** e selecione **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="d6cff-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="d6cff-120">Observação: você pode ser solicitado a reiniciar seu computador neste estágio.</span><span class="sxs-lookup"><span data-stu-id="d6cff-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="d6cff-121">Certifique-se de anotar as instruções restantes antes de reiniciar.</span><span class="sxs-lookup"><span data-stu-id="d6cff-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="d6cff-122">Abra o Gerenciador de Dispositivos novamente.</span><span class="sxs-lookup"><span data-stu-id="d6cff-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="d6cff-123">Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione Atualizar **Driver**.</span><span class="sxs-lookup"><span data-stu-id="d6cff-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="d6cff-124">Selecione **Pesquisar automaticamente para atualizar o software do driver** e siga as instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="d6cff-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>