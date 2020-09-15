---
title: Limpeza automática de dispositivos obsoletos no Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715009"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="c924c-102">Limpeza automática de dispositivos obsoletos no Intune</span><span class="sxs-lookup"><span data-stu-id="c924c-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="c924c-103">O Intune permite que o administrador configure um intervalo de tempo entre 90 e 270 dias, após o qual os dispositivos obsoletos serão removidos do serviço.</span><span class="sxs-lookup"><span data-stu-id="c924c-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="c924c-104">Essa configuração é em toda a organização e ativa o efeito imediatamente.</span><span class="sxs-lookup"><span data-stu-id="c924c-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="c924c-105">Todos os dispositivos não verificados no servidor do Intune por um período que exceda a configuração serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="c924c-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="c924c-106">**Observação** Apenas objetos de dispositivo MDM estão qualificados para essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="c924c-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="c924c-107">Os objetos de dispositivo apenas EAS são excluídos.</span><span class="sxs-lookup"><span data-stu-id="c924c-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="c924c-108">Para saber mais sobre quando um dispositivo fica qualificado para exclusão com base na configuração de limpeza do dispositivo e em seu "estado":</span><span class="sxs-lookup"><span data-stu-id="c924c-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="c924c-109">Configuração: **Excluir dispositivos após a última data de check-in: Sim (algum valor (N) em dias especificado)**</span><span class="sxs-lookup"><span data-stu-id="c924c-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="c924c-110">Com base no valor (N) definido na configuração, o serviço do Intune excluirá o dispositivo na última vez em que ele fizer check-in.</span><span class="sxs-lookup"><span data-stu-id="c924c-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="c924c-111">Configuração: **Excluir dispositivos após a última data de check-in: Não**</span><span class="sxs-lookup"><span data-stu-id="c924c-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="c924c-112">180 dias após o certificado do dispositivo expirar e não for renovado, o dispositivo será excluído.</span><span class="sxs-lookup"><span data-stu-id="c924c-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="c924c-113">**Observação** Em ambos os casos, o dispositivo deve ser registrado com êxito no Intune.</span><span class="sxs-lookup"><span data-stu-id="c924c-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="c924c-114">O registro ocorre durante o primeiro check-in de dispositivo com o serviço do Intune.</span><span class="sxs-lookup"><span data-stu-id="c924c-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="c924c-115">Se um dispositivo se inscrever com êxito para o Intune, mas não se tornar registrado em Intune, o dispositivo será excluído 270 dias após o registro.</span><span class="sxs-lookup"><span data-stu-id="c924c-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="c924c-116">(90 dias para marcar o dispositivo como revogado e, em seguida, outro 180 dias para excluir o registro.)</span><span class="sxs-lookup"><span data-stu-id="c924c-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="c924c-117">No momento, não existe nenhum mecanismo no console do Intune para estabelecer a data de vencimento da certificação de dispositivos para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c924c-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>