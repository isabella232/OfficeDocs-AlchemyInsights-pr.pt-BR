---
title: Atrasos no recebimento de alertas do SharePoint e do OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727231"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="07db8-102">Atrasos no recebimento de alertas do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="07db8-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="07db8-103">Primeiro, verifique a pasta de lixo eletrônico ou spam em seu email.</span><span class="sxs-lookup"><span data-stu-id="07db8-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="07db8-104">Se **todos os alertas de vários arquivos ou bibliotecas estiverem atrasados**, visite o [painel de integridade do serviço](https://portal.office.com/adminportal/home?ref=/servicehealth) para verificar se há avisos/incidentes que possam ocorrer com o SharePoint ou o Exchange.</span><span class="sxs-lookup"><span data-stu-id="07db8-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="07db8-105">O problema pode ser com o recurso de alerta do SharePoint ou atrasos em emails através do Exchange.</span><span class="sxs-lookup"><span data-stu-id="07db8-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="07db8-106">Observe também se outros emails estão sendo entregues, caso contrário, o problema é provavelmente com atrasos do Exchange.</span><span class="sxs-lookup"><span data-stu-id="07db8-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="07db8-107">Se **um alerta individual de um arquivo ou biblioteca específico não for entregue**, tente excluí-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="07db8-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="07db8-108">Consulte [gerenciar, exibir ou excluir alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="07db8-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="07db8-109">Não é possível enviar alertas para um grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="07db8-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="07db8-110">Só há suporte para grupos de segurança e O365.</span><span class="sxs-lookup"><span data-stu-id="07db8-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="07db8-111">Você não pode personalizar modelos de email de alerta.</span><span class="sxs-lookup"><span data-stu-id="07db8-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="07db8-112">Você deve usar o Microsoft Flow ou o fluxo de trabalho do SharePoint Designer para obtê-los.</span><span class="sxs-lookup"><span data-stu-id="07db8-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
