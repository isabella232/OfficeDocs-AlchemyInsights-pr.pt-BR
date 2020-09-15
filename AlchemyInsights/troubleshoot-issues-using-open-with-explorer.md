---
title: Solucionar problemas usando abrir com o Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659046"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="97dc8-102">Corrigir problemas com abrir com o Explorer</span><span class="sxs-lookup"><span data-stu-id="97dc8-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="97dc8-103">Correção de problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou no OneDrive usando o comando **abrir com Explorer** :</span><span class="sxs-lookup"><span data-stu-id="97dc8-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="97dc8-104">Use o Internet Explorer 10 ou o Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="97dc8-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="97dc8-105">**Abrir com o Explorer** não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="97dc8-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="97dc8-106">**Abrir com o Explorer** está desabilitado em todos os navegadores, exceto no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="97dc8-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="97dc8-107">**Abrir com o Explorer** não está disponível na experiência moderna para bibliotecas do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97dc8-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="97dc8-108">Em vez disso, use o **modo de exibição no explorador de arquivos** .</span><span class="sxs-lookup"><span data-stu-id="97dc8-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="97dc8-109">Selecione **Exibir opções** \> **Exibir no explorador de arquivos**.</span><span class="sxs-lookup"><span data-stu-id="97dc8-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="97dc8-110">O modo de exibição no explorador de arquivos não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="97dc8-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="97dc8-111">**Exibir no explorador de arquivos** somente disponível no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="97dc8-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="97dc8-112">Verifique se o serviço WebClient está em execução.</span><span class="sxs-lookup"><span data-stu-id="97dc8-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="97dc8-113">Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e pressione Enter.</span><span class="sxs-lookup"><span data-stu-id="97dc8-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="97dc8-114">Role para baixo até o serviço WebClient e verifique se a coluna **status** exibe "em execução".</span><span class="sxs-lookup"><span data-stu-id="97dc8-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="97dc8-115">Caso contrário, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="97dc8-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="97dc8-116">(Talvez seja necessário primeiro habilitar o serviço selecionando **manual** ou **automático** na caixa tipo de **inicialização** .)</span><span class="sxs-lookup"><span data-stu-id="97dc8-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="97dc8-117">A abertura de uma biblioteca no explorador de arquivos é útil se você precisar copiar ou mover vários arquivos e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos sincronizá-lo.</span><span class="sxs-lookup"><span data-stu-id="97dc8-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="97dc8-118">Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="97dc8-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="97dc8-119">Para obter informações sobre como configurar a sincronização, consulte [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="97dc8-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="97dc8-120">Confira o artigo [como usar o comando "abrir com o Explorer" para solucionar problemas no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="97dc8-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

