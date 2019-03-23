---
title: Solucionar problemas usando abrir com o Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759282"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="796a9-102">Corrigir problemas com abrir com o Explorer</span><span class="sxs-lookup"><span data-stu-id="796a9-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="796a9-103">Correção de problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou no OneDrive usando o comando **abrir com Explorer** :</span><span class="sxs-lookup"><span data-stu-id="796a9-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="796a9-104">Use o Internet Explorer 10 ou o Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="796a9-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="796a9-105">**Abrir com o Explorer** não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="796a9-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="796a9-106">**Abrir com o Explorer** está desabilitado em todos os navegadores, exceto no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="796a9-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="796a9-107">**Abrir com o Explorer** não está disponível na experiência moderna para bibliotecas do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="796a9-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="796a9-108">Em vez disso, use o **modo de exibição no explorador de arquivos** .</span><span class="sxs-lookup"><span data-stu-id="796a9-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="796a9-109">Selecione **Exibir opções** \> **Exibir no explorador de arquivos**.</span><span class="sxs-lookup"><span data-stu-id="796a9-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="796a9-110">O modo de exibição no explorador de arquivos não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="796a9-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="796a9-111">**Exibir no explorador de arquivos** somente disponível no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="796a9-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="796a9-112">Verifique se o serviço webClient está em execução.</span><span class="sxs-lookup"><span data-stu-id="796a9-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="796a9-113">Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e pressione Enter.</span><span class="sxs-lookup"><span data-stu-id="796a9-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="796a9-114">Role para baixo até o serviço webClient e verifique se a coluna **status** exibe "em execução".</span><span class="sxs-lookup"><span data-stu-id="796a9-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="796a9-115">Caso contrário, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="796a9-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="796a9-116">(Talvez seja necessário primeiro habilitar o serviço selecionando **manual** ou **automático** na caixa tipo de **inicialização** .)</span><span class="sxs-lookup"><span data-stu-id="796a9-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="796a9-117">A abertura de uma biblioteca no explorador de arquivos é útil se você precisar copiar ou mover vários arquivos e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos sincronizá-lo.</span><span class="sxs-lookup"><span data-stu-id="796a9-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="796a9-118">Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="796a9-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="796a9-119">Para obter informações sobre como configurar a sincronização, consulte [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="796a9-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="796a9-120">Confira o artigo [como usar o comando "abrir com o Explorer" para solucionar problemas no SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="796a9-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

