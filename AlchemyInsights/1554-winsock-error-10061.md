---
title: Erro de Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274480"
---
# <a name="winsock-error-10061"></a>Erro de Winsock 10061

Este código de erro significa que o Office 365 não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas configurações:
  
- Verificar a configuração de firewall com as informações em [URLs do Office 365 e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Se o erro é específico ao Exchange Online Protection (EOP), você deve foram anteriormente notificados para uma alteração para os [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.
    
- Verifique se as configurações do servidor host e destino inteligentes em seus conectores.
    
Observe que o Office 365 não bloqueie as conexões de *entrada* dessa maneira. 
  

