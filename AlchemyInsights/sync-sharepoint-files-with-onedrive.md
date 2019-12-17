---
title: Solucionar problemas de "Abrir com o Explorer" no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050801"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="758b8-102">Solucionar problemas de "Abrir com o Explorer" no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="758b8-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="758b8-103">O comando Abrir com o Explorer abre uma instância local do Windows Explorer que exibe a estrutura de pastas no servidor que hospeda o site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="758b8-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="758b8-104">Dito isto, recomendamos que você [sincronize os arquivos do SharePoint com o novo cliente de sincronização do OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, que fornece o [Arquivos Sob Demanda](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) porque ele fornece acesso local aos seus arquivos e oferece o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="758b8-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="758b8-105">Se você optou por usar a Exibição do Explorer em vez de usar o novo cliente de sincronização do OneDrive, siga as etapas e as práticas recomendadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="758b8-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="758b8-106">Como usar o comando "Abrir com o Explorer" para solucionar problemas no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="758b8-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="758b8-107">Copiar ou mover arquivos de biblioteca usando a opção Abrir com o Explorador</span><span class="sxs-lookup"><span data-stu-id="758b8-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="758b8-108">O botão **Abrir com o Explorer** não aparece na nova experiência de biblioteca.</span><span class="sxs-lookup"><span data-stu-id="758b8-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="758b8-109">Selecione o menu suspenso **Exibir** no canto superior direito (o nome do menu suspenso varia dependendo da sua exibição atual), e, então, selecione **Exibir no Explorador de Arquivos**.</span><span class="sxs-lookup"><span data-stu-id="758b8-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="758b8-110">O recurso do SharePoint Abrir com o Explorer usa controles ActiveX, portanto, é compatível apenas com o Internet Explorer 10 ou 11.</span><span class="sxs-lookup"><span data-stu-id="758b8-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="758b8-111">Abrir com o Explorer não funciona no Windows com o Microsoft Edge, Google Chrome ou Mozilla Firefox, ou na plataforma Mac.</span><span class="sxs-lookup"><span data-stu-id="758b8-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="758b8-112">Devido a esse motivo, a opção Exibição do Explorer pode estar desativada.</span><span class="sxs-lookup"><span data-stu-id="758b8-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="758b8-113">[Por que os botões da faixa de opções do SharePoint não estão disponíveis ou estão esmaecidos](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="758b8-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

