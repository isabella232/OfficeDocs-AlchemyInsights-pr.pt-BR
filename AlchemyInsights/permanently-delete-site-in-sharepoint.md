---
title: Excluir permanentemente um site no SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944299"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Excluir permanentemente um site no SharePoint

Para reutilizar uma URL de um site excluído (para recriar um site) ou excluir um site permanentemente porque ele não é mais usado, você pode usar **Excluir permanentemente** do novo Centro de administração do SharePoint. 

1. Vá para a [página Sites excluídos do novo centro de administração do SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e entre com uma conta que tenha permissões de administrador para sua organização. 

2. Na coluna da esquerda, selecione um site. 

3. Clique em **Excluir permanentemente.**. 

**Observação**: os sites conectados ao grupo não podem ser excluídos permanentemente do Novo Centro de Administração do SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) precisará ser usado no lugar.  

Para obter mais informações, consulte [Excluir permanentemente um site.](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
