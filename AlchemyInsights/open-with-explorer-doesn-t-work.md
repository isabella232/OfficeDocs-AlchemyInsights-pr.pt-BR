---
title: Abrir com o Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419849"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="a6b26-102">Abrir com o Explorer não está funcionando</span><span class="sxs-lookup"><span data-stu-id="a6b26-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="a6b26-103">Se **Open com Explorer** ou **View no explorador de arquivos** não funcionar, certifique-se de que o serviço WebClient está definido para **executar** seguindo as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="a6b26-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="a6b26-104">Por exemplo, pode levar muito tempo para abrir uma biblioteca do SharePoint ou do OneDrive quando o serviço não estiver em execução.</span><span class="sxs-lookup"><span data-stu-id="a6b26-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="a6b26-105">Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e selecione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a6b26-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="a6b26-106">Role para baixo até o serviço webClient e verifique a coluna **status** .</span><span class="sxs-lookup"><span data-stu-id="a6b26-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="a6b26-107">Se o status do serviço webClient não estiver **em execução**, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6b26-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a6b26-108">Habilite o serviço, se necessário, selecionando **manual** ou **automático** na caixa **tipo de inicialização** .</span><span class="sxs-lookup"><span data-stu-id="a6b26-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a6b26-109">Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a6b26-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a6b26-110">Explorar a sincronização como uma alternativa melhor: [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a6b26-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

