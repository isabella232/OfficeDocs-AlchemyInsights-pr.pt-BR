---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551439"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="37e19-102">Restringir o acesso no SharePoint ou no OneDrive</span><span class="sxs-lookup"><span data-stu-id="37e19-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="37e19-103">No SharePoint e no OneDrive, você restringe o acesso a itens como arquivos, pastas e listas concedendo acesso somente a grupos ou pessoas aos quais você deseja ter acesso.</span><span class="sxs-lookup"><span data-stu-id="37e19-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="37e19-104">Por padrão, as permissões no SharePoint são herdadas da parte superior na hierarquia.</span><span class="sxs-lookup"><span data-stu-id="37e19-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="37e19-105">Portanto, um arquivo herda suas permissões da pasta, que herda suas permissões da biblioteca, que herda suas permissões do site.</span><span class="sxs-lookup"><span data-stu-id="37e19-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="37e19-106">Você pode compartilhar em um nível superior (por exemplo, compartilhar um site inteiro) e, em seguida, interromper a herança se não quiser compartilhar todos os itens no site.</span><span class="sxs-lookup"><span data-stu-id="37e19-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="37e19-107">No entanto, não recomendamos isso, pois ela torna a manutenção das permissões mais complexa e confusa no futuro.</span><span class="sxs-lookup"><span data-stu-id="37e19-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="37e19-108">Veja o que você pode fazer em vez disso:</span><span class="sxs-lookup"><span data-stu-id="37e19-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="37e19-109">Se, por exemplo, você quiser compartilhar todo o conteúdo de uma pasta, exceto para um arquivo nele, mova esse arquivo para um novo local que não seja compartilhado.</span><span class="sxs-lookup"><span data-stu-id="37e19-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="37e19-110">Se você tiver duas subpastas em uma pasta e quiser compartilhar uma subpasta com grupos A e B e permitir apenas o grupo um acesso à segunda subpasta, compartilhe a pasta pai com o grupo A e adicione o grupo B à primeira subpasta.</span><span class="sxs-lookup"><span data-stu-id="37e19-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="37e19-111">Parar de compartilhar um arquivo ou uma pasta</span><span class="sxs-lookup"><span data-stu-id="37e19-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

