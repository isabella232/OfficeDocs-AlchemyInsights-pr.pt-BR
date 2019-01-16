---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274969"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou OneDrive

No SharePoint e OneDrive, você restringir o acesso a itens como arquivos, pastas e listas, concedendo acesso somente aos grupos ou indivíduos que você deseja que tenham acesso. Por padrão, as permissões no SharePoint são herdadas da up superior na hierarquia. Portanto, um arquivo herda suas permissões da pasta, que herda suas permissões da biblioteca, o qual herda suas permissões do site.
  
Você pode compartilhar em um nível superior (como compartilhando um site inteiro) e interromper a herança, se você não deseja compartilhar todos os itens no site. No entanto, não recomendamos isso porque torna a manter as permissões mais complexa e confusa no futuro. Aqui está o que você pode fazer em vez disso:
  
- Se, por exemplo, você deseja compartilhar todo o conteúdo de uma pasta, com exceção de um arquivo nela, mova esse arquivo para um novo local que não é compartilhado.
    
- Se você tiver duas subpastas em uma pasta, e você deseja compartilhar uma subpasta com grupos A e B e permitir o acesso de grupo A apenas para a segunda subpasta, compartilhe a pasta pai com grupo A e adicionar o grupo B para a subpasta primeira.
    
[Parar de compartilhar um arquivo ou pasta](https://go.microsoft.com/fwlink/?linkid=2008861)
  

