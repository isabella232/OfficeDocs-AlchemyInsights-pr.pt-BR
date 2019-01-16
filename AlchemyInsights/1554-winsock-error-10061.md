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
# <a name="winsock-error-10061"></a><span data-ttu-id="459e4-102">Erro de Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="459e4-102">Winsock error 10061</span></span>

<span data-ttu-id="459e4-p101">Este código de erro significa que o Office 365 não pôde estabelecer um soquete TCP (conexão) com o host de destino. A causa mais provável desse erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas configurações:</span><span class="sxs-lookup"><span data-stu-id="459e4-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="459e4-106">Verificar a configuração de firewall com as informações em [URLs do Office 365 e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="459e4-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="459e4-107">Se o erro é específico ao Exchange Online Protection (EOP), você deve foram anteriormente notificados para uma alteração para os [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="459e4-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="459e4-108">Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.</span><span class="sxs-lookup"><span data-stu-id="459e4-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="459e4-109">Verifique se as configurações do servidor host e destino inteligentes em seus conectores.</span><span class="sxs-lookup"><span data-stu-id="459e4-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="459e4-110">Observe que o Office 365 não bloqueie as conexões de *entrada* dessa maneira.</span><span class="sxs-lookup"><span data-stu-id="459e4-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

