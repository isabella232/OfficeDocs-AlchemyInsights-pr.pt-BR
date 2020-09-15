---
title: Localizando dispositivos iOS perdidos com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675143"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="3d9d2-102">Localizando dispositivos iOS perdidos com o Intune</span><span class="sxs-lookup"><span data-stu-id="3d9d2-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="3d9d2-103">Habilitar o modo de perda em um dispositivo iOS permite que um administrador tenha uma mensagem e o número de telefone de contato exibido na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="3d9d2-104">Após o modo de perda ser habilitado, o administrador pode usar a ação localizar dispositivo para identificar o local físico do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="3d9d2-105">A ação Localizar dispositivo no Intune funciona com dispositivos iOS para mostrar o local de um dispositivo específico em um mapa.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="3d9d2-106">Usar essa ação requer que o dispositivo iOS esteja no:</span><span class="sxs-lookup"><span data-stu-id="3d9d2-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="3d9d2-107">Modo supervisionado</span><span class="sxs-lookup"><span data-stu-id="3d9d2-107">Supervised mode</span></span>
- <span data-ttu-id="3d9d2-108">Modo perdido</span><span class="sxs-lookup"><span data-stu-id="3d9d2-108">Lost mode</span></span>

<span data-ttu-id="3d9d2-109">Para saber mais, confira [Habilitar o modo perdido em dispositivos iOS/iPadOS com o Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Localizar dispositivos iOS/iPadOS perdidos ou roubados com o Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="3d9d2-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="3d9d2-110">**Perguntas Frequentes**</span><span class="sxs-lookup"><span data-stu-id="3d9d2-110">**FAQ**</span></span>

<span data-ttu-id="3d9d2-111">P: Efetuei uma ação remota para remover dados da empresa de um dispositivo, mas agora ele está travado em um estado pendente.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="3d9d2-112">R: Para que uma ação remota seja concluída com sucesso, o dispositivo de destino precisa estar online e íntegro.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="3d9d2-113">Nas situações a seguir, a ação remota permanece em um estado pendente por 30 dias ou até que o dispositivo confirme o comando:</span><span class="sxs-lookup"><span data-stu-id="3d9d2-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="3d9d2-114">Quando o dispositivo não tem conectividade</span><span class="sxs-lookup"><span data-stu-id="3d9d2-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="3d9d2-115">Quando o dispositivo perder seu status de gerenciamento com o Intune</span><span class="sxs-lookup"><span data-stu-id="3d9d2-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="3d9d2-116">Se você acha que um dispositivo não está mais fazendo check-in do e que não poderá remover dados da empresa, selecione Excluir.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="3d9d2-117">A exclusão irá remover o registro do dispositivo e ele não aparecerá mais na lista de dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="3d9d2-118">Se o dispositivo se tornar ativo novamente, o usuário precisará registrá-lo novamente.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="3d9d2-119">P: Por que determinadas ações remotas não estão disponíveis para uso?</span><span class="sxs-lookup"><span data-stu-id="3d9d2-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="3d9d2-120">R: Nem todas as plataformas são compatíveis com todas as ações remotas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="3d9d2-121">As seguintes ações remotas são específicas de uma plataforma, para que elas fiquem disponíveis apenas para as plataformas indicadas.</span><span class="sxs-lookup"><span data-stu-id="3d9d2-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="3d9d2-122">Ignorar bloqueio de ativação (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="3d9d2-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="3d9d2-123">Novo Início (somente Windows)</span><span class="sxs-lookup"><span data-stu-id="3d9d2-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="3d9d2-124">Modo perdido (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="3d9d2-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="3d9d2-125">Localizar dispositivo (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="3d9d2-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="3d9d2-126">Reiniciar (somente Windows)</span><span class="sxs-lookup"><span data-stu-id="3d9d2-126">Restart (Windows only)</span></span>

<span data-ttu-id="3d9d2-127">Para obter mais detalhes sobre cada uma dessas ações, confira o artigo [Ações disponíveis para dispositivos](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="3d9d2-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>