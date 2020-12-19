---
title: Remover versões anteriores do MSI do Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680589"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="45275-102">Remover versões anteriores do MSI do Office</span><span class="sxs-lookup"><span data-stu-id="45275-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="45275-103">Recomendo a remoção de versões anteriores do Windows Installer (MSI) do Office antes de instalar o Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="45275-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="45275-104">Confira aqui como fazer isso:</span><span class="sxs-lookup"><span data-stu-id="45275-104">Here's how to do this:</span></span>

1. <span data-ttu-id="45275-105">Se você usou o MSI para instalar o Office, poderá usar a ferramenta de implantação do Office (ODT) para desinstalar o Office.</span><span class="sxs-lookup"><span data-stu-id="45275-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="45275-106">Você pode usar o elemento RemoveMSI no arquivo **configuration.xml** .</span><span class="sxs-lookup"><span data-stu-id="45275-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="45275-107">Siga as instruções deste artigo: [centro de conformidade & segurança do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="45275-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>