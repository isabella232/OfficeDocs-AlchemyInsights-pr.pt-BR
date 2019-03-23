---
title: 1554 erro do Winsock 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772430"
---
# <a name="winsock-error-10061"></a>Erro do Winsock 10061

Esse código de erro significa que o Office 365 não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, Confira estas configurações:
  
- Verificar a configuração do firewall com as informações nas [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Se o erro for específico para o proteção do Exchange Online (EOP), você deverá ter sido notificado anteriormente sobre uma alteração nos [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.
    
- Verifique as configurações de host inteligente e servidor de destino em seus conectores.
    
Observe que o Office 365 não bloqueia conexões de *entrada* dessa maneira. 
  

