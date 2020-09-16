---
title: Problemas de conexão do SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727159"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="26487-102">Problemas de conexão do SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="26487-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="26487-103">Se o SharePoint Designer estiver enfrentando problemas de conexão para sites do SharePoint, tente as soluções comuns a seguir.</span><span class="sxs-lookup"><span data-stu-id="26487-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="26487-104">Etapa 1: verificar se o SharePoint Designer 2013 foi atualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a [atualização de 2 de agosto de 2016 para o SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="26487-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="26487-105">Etapa 2: limpar os arquivos de cache local:</span><span class="sxs-lookup"><span data-stu-id="26487-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="26487-106">Feche o SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="26487-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="26487-107">No computador local, remova todos os arquivos encontrados em cada uma das pastas a seguir.</span><span class="sxs-lookup"><span data-stu-id="26487-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="26487-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="26487-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="26487-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="26487-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="26487-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="26487-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="26487-111">Abra o SharePoint Designer 2013 e insira a conta novamente para ver se ele funciona.</span><span class="sxs-lookup"><span data-stu-id="26487-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="26487-112">Etapa 3: [habilitar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="26487-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="26487-113">Etapa 4: os administradores precisarão **permitir o script personalizado** nas configurações do centro de administração do SharePoint para permitir a conexão com o SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="26487-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="26487-114">Consulte [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="26487-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


