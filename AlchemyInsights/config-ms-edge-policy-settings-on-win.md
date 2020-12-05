---
title: Definir configurações de política do Microsoft Edge no Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576334"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="b970f-102">Definir configurações de política do Microsoft Edge no Windows</span><span class="sxs-lookup"><span data-stu-id="b970f-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="b970f-103">Para definir configurações de política e atualizações gerenciadas para o Microsoft Edge, use objetos de política de grupo (GPOs).</span><span class="sxs-lookup"><span data-stu-id="b970f-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="b970f-104">Você também pode provisionar a política pelo registro; Isso seria apropriado para (1) dispositivos Windows que ingressaram em um domínio do Microsoft Active Directory e para (2) instâncias do Windows 10 pro e Enterprise registradas para o gerenciamento de dispositivos no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="b970f-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="b970f-105">Para configurar o Microsoft Edge usando GPOs, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="b970f-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="b970f-106">Para o repositório central de política de grupo no seu domínio do Active Directory ou para a pasta de modelo de definição de política em computadores individuais, instale todos os modelos administrativos que adicionam regras e configurações para o Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b970f-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="b970f-107">Configure as políticas específicas que você deseja definir.</span><span class="sxs-lookup"><span data-stu-id="b970f-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="b970f-108">Para saber mais, confira [configurar as configurações de política do Microsoft Edge no Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="b970f-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
