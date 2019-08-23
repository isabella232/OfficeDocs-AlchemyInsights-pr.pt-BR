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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

No SharePoint e no OneDrive, você restringe o acesso a itens como arquivos, pastas e listas concedendo acesso somente a grupos ou pessoas aos quais você deseja ter acesso. Por padrão, as permissões no SharePoint são herdadas da parte superior na hierarquia. Portanto, um arquivo herda suas permissões da pasta, que herda suas permissões da biblioteca, que herda suas permissões do site.
  
Você pode compartilhar em um nível superior (por exemplo, compartilhar um site inteiro) e, em seguida, interromper a herança se não quiser compartilhar todos os itens no site. No entanto, não recomendamos isso, pois ela torna a manutenção das permissões mais complexa e confusa no futuro. Veja o que você pode fazer em vez disso:
  
- Se, por exemplo, você quiser compartilhar todo o conteúdo de uma pasta, exceto para um arquivo nele, mova esse arquivo para um novo local que não seja compartilhado.
    
- Se você tiver duas subpastas em uma pasta e quiser compartilhar uma subpasta com grupos A e B e permitir apenas o grupo um acesso à segunda subpasta, compartilhe a pasta pai com o grupo A e adicione o grupo B à primeira subpasta.
    
[Parar de compartilhar um arquivo ou uma pasta](https://go.microsoft.com/fwlink/?linkid=2008861)
  

