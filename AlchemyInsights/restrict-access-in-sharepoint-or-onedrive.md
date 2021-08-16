---
title: Restringir o acesso em SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075028"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso em SharePoint ou OneDrive

Em SharePoint e OneDrive, você restringe o acesso a itens como arquivos, pastas e listas, concedendo acesso apenas a grupos ou indivíduos que você deseja ter acesso. Por padrão, as permissões SharePoint são herdadas de superiores na hierarquia. Portanto, um arquivo herda suas permissões da pasta, que herda suas permissões da biblioteca, que herda suas permissões do site.
  
Você pode compartilhar em um nível mais alto (por exemplo, compartilhando um site inteiro) e, em seguida, quebrar a herança se não quiser compartilhar todos os itens no site. No entanto, não recomendamos isso porque isso torna a manutenção das permissões mais complexa e confusa no futuro. Veja o que você poderia fazer em vez disso:
  
- Se, por exemplo, você quiser compartilhar todo o conteúdo de uma pasta, exceto um arquivo, mova esse arquivo para um novo local que não seja compartilhado.
    
- Se você tiver duas subpastas em uma pasta e quiser compartilhar uma subpasta com os grupos A e B e permitir apenas o acesso do grupo A à segunda subpasta, compartilhe a pasta pai com o grupo A e adicione o grupo B à primeira subpasta.
    
[Parar de compartilhar um arquivo ou pasta ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

