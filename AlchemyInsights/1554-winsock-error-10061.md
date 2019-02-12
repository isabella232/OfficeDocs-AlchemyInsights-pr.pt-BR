---
title: Erro de Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903084"
---
# <a name="winsock-error-10061"></a>Erro de Winsock 10061

Este código de erro significa que o Office 365 não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas configurações:
  
- Verificar a configuração de firewall com as informações em [URLs do Office 365 e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Se o erro é específico ao Exchange Online Protection (EOP), você deve foram anteriormente notificados para uma alteração para os [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.
    
- Verifique se as configurações do servidor host e destino inteligentes em seus conectores.
    
Observe que o Office 365 não bloqueie as conexões de *entrada* dessa maneira. 
  

