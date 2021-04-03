---
title: Restaurar um grupo excluído do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505669"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="5d7b2-102">Restaurar um grupo excluído do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5d7b2-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="5d7b2-103">Você pode restaurar um grupo excluído do Microsoft 365 ou o Microsoft Teams dentro de 30 dias a partir da exclusão.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="5d7b2-104">Para fazer logon no Centro de administração do Microsoft 365 e listar os grupos e equipes excluídos, vá para o Centro de administração [do Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="5d7b2-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="5d7b2-105">**Observação:** Faça logoff usando a conta atribuída ao administrador do locatário ou à função de administrador de grupos.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="5d7b2-106">Selecione o grupo/Teams excluído do Microsoft 365 a ser restaurado e clique em **restaurar o grupo**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="5d7b2-107">Se o grupo não puder ser restaurado devido a um endereço SMTP conflitante, use o seguinte comando para encontrar o objeto que está causando conflito e remover o endereço SMTP:</span><span class="sxs-lookup"><span data-stu-id="5d7b2-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="5d7b2-108">**Observação:** Em alguns casos, pode levar até 24 horas para que o grupo e todos os seus dados sejam restaurados.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="5d7b2-109">Para obter mais informações ou saber como restaurar grupos usando o PowerShell, consulte [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="5d7b2-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>