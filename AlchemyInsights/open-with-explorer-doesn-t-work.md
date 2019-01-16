---
title: Abrir com Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274179"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="2768c-102">Abrir com Explorer não está funcionando</span><span class="sxs-lookup"><span data-stu-id="2768c-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="2768c-p101">Se **Abrir com Explorer** ou **modo de exibição no Gerenciador de arquivos** não funcionar, verifique se que o serviço de cliente está definido para **execução** seguindo as etapas abaixo. Por exemplo, ela pode levar muito tempo para abrir uma biblioteca do SharePoint ou OneDrive quando o serviço não está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="2768c-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="2768c-105">Na caixa de pesquisa do Windows, digite executar, selecione o aplicativo da área de trabalho, Services. msc do tipo e selecione **Enter**a executar.</span><span class="sxs-lookup"><span data-stu-id="2768c-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="2768c-p102">Role para baixo até o serviço de cliente e verifique a coluna **Status** . Se o status do serviço de cliente não estiver **em execução**, clique duas vezes em serviço, clique em **Iniciar**e, em seguida, clique em **Okey**. Habilite o serviço, se necessário, selecionando **Manual** ou **automático** na caixa **tipo de inicialização** .</span><span class="sxs-lookup"><span data-stu-id="2768c-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2768c-p103">Para solucionar problemas de abertura no Gerenciador de arquivos, consulte [Abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore a sincronização como uma alternativa melhor: [arquivos de sincronização do SharePoint com o novo cliente de sincronização do OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2768c-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

