---
title: 1554 Erro winsock 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083218"
---
# <a name="winsock-error-10061"></a>Erro Winsock 10061

Esse código de erro significa que a Microsoft não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas configurações:

- Verifique a configuração do firewall com as informações [em Microsoft 365 URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se o erro for específico para Proteção do Exchange Online (EOP), você deve ter sido notificado anteriormente para uma alteração nos endereços IP Proteção do Exchange Online [ip](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifique se o Provedor de Serviços da Internet (ISP) não está bloqueando a porta.

- Verifique as configurações do host inteligente e do servidor de destino em seus conectores.

Observe que Microsoft 365 não bloqueia *conexões de* entrada dessa maneira.
