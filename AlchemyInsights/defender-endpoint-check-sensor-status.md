---
title: Status do sensor de verificação do Ponto de Extremidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627225"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="883d5-102">Status do sensor de verificação do Ponto de Extremidade</span><span class="sxs-lookup"><span data-stu-id="883d5-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="883d5-103">O bloco **Dispositivos com problemas de sensor** está localizado no painel Operações de Segurança.</span><span class="sxs-lookup"><span data-stu-id="883d5-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="883d5-104">Este bloco fornece informações sobre a capacidade do dispositivo individual de fornecer dados do sensor e se comunicar com o serviço Ponto de Extremidade.</span><span class="sxs-lookup"><span data-stu-id="883d5-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="883d5-105">Ele relata quantos dispositivos requerem atenção e ajuda a identificar dispositivos problemáticos e tomar medidas para corrigir os problemas conhecidos.</span><span class="sxs-lookup"><span data-stu-id="883d5-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="883d5-106">Dois indicadores de status no bloco fornecem informações sobre o número de dispositivos que não se reportam adequadamente ao serviço:</span><span class="sxs-lookup"><span data-stu-id="883d5-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="883d5-107">Dispositivos **Misconfigured** que podem estar relatando dados do sensor parcialmente ao serviço de Ponto de Extremidade e podem ter erros de configuração que precisam ser corrigidos.</span><span class="sxs-lookup"><span data-stu-id="883d5-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="883d5-108">Dispositivos **Inativos** que pararam de se reportar ao serviço de Ponto de Extremidade por mais de sete dias no mês anterior.</span><span class="sxs-lookup"><span data-stu-id="883d5-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="883d5-109">Clicar em qualquer um dos grupos direciona você para a lista de dispositivos, filtrada de acordo com suas escolhas.</span><span class="sxs-lookup"><span data-stu-id="883d5-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="883d5-110">Na lista de dispositivos, você pode filtrar a lista de estado de integridade pelo seguinte status:</span><span class="sxs-lookup"><span data-stu-id="883d5-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="883d5-111">Dispositivos **ativos** que estão se reportando ativamente ao serviço de Ponto de Extremidade.</span><span class="sxs-lookup"><span data-stu-id="883d5-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="883d5-112">Dispositivos **Misconfigured** que podem estar relatando parcialmente os dados do sensor ao serviço de Ponto de Extremidade, mas têm erros de configuração que precisam ser corrigidos.</span><span class="sxs-lookup"><span data-stu-id="883d5-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="883d5-113">Dispositivos mal configurados podem ter um ou uma combinação dos seguintes problemas:</span><span class="sxs-lookup"><span data-stu-id="883d5-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="883d5-114">Sem dados do sensor - os dispositivos pararam de enviar dados do sensor.</span><span class="sxs-lookup"><span data-stu-id="883d5-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="883d5-115">Alertas limitados podem ser acionados a partir do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="883d5-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="883d5-116">Comunicações prejudicadas - A capacidade de comunicação com o dispositivo está prejudicada.</span><span class="sxs-lookup"><span data-stu-id="883d5-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="883d5-117">O envio de arquivos para análise profunda, bloqueio de arquivos, isolamento do dispositivo da rede e outras ações que exigem comunicação com o dispositivo podem não funcionar.</span><span class="sxs-lookup"><span data-stu-id="883d5-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="883d5-118">Dispositivos **Inativos** que pararam de se reportar ao serviço de Ponto de Extremidade.</span><span class="sxs-lookup"><span data-stu-id="883d5-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="883d5-119">Você pode baixar a lista inteira em formato CSV usando o recurso Exportar.</span><span class="sxs-lookup"><span data-stu-id="883d5-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="883d5-120">Para obter mais informações, confira [Verificar o estado de integridade do sensor no Microsoft Defender para Ponto de Extremidade](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="883d5-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="883d5-121">Para obter mais informações sobre o que fez com que um dispositivo ficasse inativo ou configurado incorretamente, confira [Corrigir sensores não íntegros no Microsoft Defender para Ponto de Extremidade](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="883d5-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
