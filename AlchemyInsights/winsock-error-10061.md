---
title: 1554 erro do Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698850"
---
# <a name="winsock-error-10061"></a>Erro do Winsock 10061

Esse código de erro significa que a Microsoft não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, Confira estas configurações:

- Verificar a configuração do firewall com as informações nas [URLs e intervalos de endereços IP do Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se o erro for específico para o proteção do Exchange Online (EOP), você deverá ter sido notificado anteriormente sobre uma alteração nos [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.

- Verifique as configurações de host inteligente e servidor de destino em seus conectores.

Observe que o Microsoft 365 não bloqueia conexões de *entrada* dessa maneira.
