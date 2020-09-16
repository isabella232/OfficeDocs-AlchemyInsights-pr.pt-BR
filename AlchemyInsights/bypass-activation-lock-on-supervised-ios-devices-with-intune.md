---
title: Ignorar o bloqueio de ativação em dispositivos iOS supervisionados com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757288"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="d144f-102">Ignorar o bloqueio de ativação em dispositivos iOS supervisionados com o Intune</span><span class="sxs-lookup"><span data-stu-id="d144f-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="d144f-103">A capacidade de ignorar o bloqueio de ativação nos dispositivos iOS torna mais fácil a recuperação de uma situação na qual um usuário habilita a ativação do bloqueio em um dispositivo corporativo e, em seguida, sai da empresa.</span><span class="sxs-lookup"><span data-stu-id="d144f-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="d144f-104">Os pré-requisitos para se ignorar uma ativação de bloqueio incluem:</span><span class="sxs-lookup"><span data-stu-id="d144f-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="d144f-105">Um dispositivo que seja “supervisionado”.</span><span class="sxs-lookup"><span data-stu-id="d144f-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="d144f-106">Um bloqueio de ativação habilitado com sucesso usando a política de restrições de dispositivos iOS no Intune.</span><span class="sxs-lookup"><span data-stu-id="d144f-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="d144f-107">Além disso, ao ignorar um bloqueio de ativação você deve:</span><span class="sxs-lookup"><span data-stu-id="d144f-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="d144f-108">Ter em mãos (posse física) o dispositivo que está sendo apagado.</span><span class="sxs-lookup"><span data-stu-id="d144f-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="d144f-109">Copiar o código antes de efetivar o apagamento.</span><span class="sxs-lookup"><span data-stu-id="d144f-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="d144f-110">**Observação:** o código de apagamento não diferencia maiúsculas e minúsculas e, portanto, os caracteres "-" não são necessários.</span><span class="sxs-lookup"><span data-stu-id="d144f-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="d144f-111">Para obter mais detalhes, confira o artigo [Ignorar bloqueios de ativação em dispositivos iOS supervisionados com o Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="d144f-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="d144f-112">**Perguntas Frequentes**</span><span class="sxs-lookup"><span data-stu-id="d144f-112">**FAQ**</span></span>

<span data-ttu-id="d144f-113">P: **Efetuei uma ação remota para remover dados da empresa de um dispositivo, mas agora ele está travado em um estado pendente.**</span><span class="sxs-lookup"><span data-stu-id="d144f-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="d144f-114">R: Para que uma ação remota seja concluída com sucesso, o dispositivo de destino precisa estar online e íntegro.</span><span class="sxs-lookup"><span data-stu-id="d144f-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="d144f-115">Nas situações a seguir, a ação remota permanece em estado pendente por 30 dias ou até que o dispositivo confirme o comando, sempre que o dispositivo:</span><span class="sxs-lookup"><span data-stu-id="d144f-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="d144f-116">Estiver sem conexão.</span><span class="sxs-lookup"><span data-stu-id="d144f-116">Does not have connectivity.</span></span>
- <span data-ttu-id="d144f-117">Perder seu status de gerenciamento no Intune.</span><span class="sxs-lookup"><span data-stu-id="d144f-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="d144f-118">Se você acredita que um dispositivo não está mais tendo acesso e não será capaz de remover os dados da empresa, selecione Excluir.</span><span class="sxs-lookup"><span data-stu-id="d144f-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="d144f-119">A exclusão irá remover o registro do dispositivo e ele não aparecerá mais na lista de dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="d144f-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="d144f-120">Para que o dispositivo se torne ativo novamente, seu usuário precisará recadastrá-lo.</span><span class="sxs-lookup"><span data-stu-id="d144f-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="d144f-121">P: **Por que determinadas ações remotas não estão disponíveis para uso?**</span><span class="sxs-lookup"><span data-stu-id="d144f-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="d144f-122">R: Nem todas as plataformas são compatíveis com todas as ações remotas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d144f-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="d144f-123">As ações remotas a seguir são específicas para uma plataforma:</span><span class="sxs-lookup"><span data-stu-id="d144f-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="d144f-124">Ignorar bloqueio de ativação (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="d144f-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="d144f-125">Novo Início (somente Windows)</span><span class="sxs-lookup"><span data-stu-id="d144f-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="d144f-126">Modo perdido (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="d144f-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="d144f-127">Localizar dispositivo (somente iOS)</span><span class="sxs-lookup"><span data-stu-id="d144f-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="d144f-128">Reiniciar (somente Windows)</span><span class="sxs-lookup"><span data-stu-id="d144f-128">Restart (Windows only)</span></span>

<span data-ttu-id="d144f-129">Para obter mais detalhes sobre cada uma dessas ações, confira o artigo [Ações disponíveis para dispositivos](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="d144f-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>