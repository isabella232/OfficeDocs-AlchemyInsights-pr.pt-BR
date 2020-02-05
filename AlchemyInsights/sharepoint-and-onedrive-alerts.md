---
title: Atrasos no recebimento de alertas do SharePoint e do OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771203"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="e2831-102">Atrasos no recebimento de alertas do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="e2831-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="e2831-103">Primeiro, verifique a pasta de lixo eletrônico ou spam em seu email.</span><span class="sxs-lookup"><span data-stu-id="e2831-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="e2831-104">Se **todos os alertas de vários arquivos ou bibliotecas estiverem atrasados**, visite o [painel de integridade do serviço](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) para verificar se há avisos/incidentes que possam ocorrer com o SharePoint ou o Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2831-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="e2831-105">O problema pode ser com o recurso de alerta do SharePoint ou atrasos em emails através do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2831-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="e2831-106">Observe também se outros emails estão sendo entregues, caso contrário, o problema é provavelmente com atrasos do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2831-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="e2831-107">Se **um alerta individual de um arquivo ou biblioteca específico não for entregue**, tente excluí-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="e2831-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="e2831-108">Consulte [gerenciar, exibir ou excluir alertas do SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="e2831-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="e2831-109">Não é possível enviar alertas para um grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e2831-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="e2831-110">Só há suporte para grupos de segurança e O365.</span><span class="sxs-lookup"><span data-stu-id="e2831-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="e2831-111">Você não pode personalizar modelos de email de alerta.</span><span class="sxs-lookup"><span data-stu-id="e2831-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="e2831-112">Você deve usar o Microsoft Flow ou o fluxo de trabalho do SharePoint Designer para obtê-los.</span><span class="sxs-lookup"><span data-stu-id="e2831-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
