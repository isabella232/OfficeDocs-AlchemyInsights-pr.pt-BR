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
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859128"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="ee716-102">Erro do Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="ee716-102">Winsock error 10061</span></span>

<span data-ttu-id="ee716-103">Esse código de erro significa que o Office 365 não pôde estabelecer um soquete TCP (conexão) com o host de destino.</span><span class="sxs-lookup"><span data-stu-id="ee716-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="ee716-104">A causa mais provável desse erro é um problema com a configuração do firewall.</span><span class="sxs-lookup"><span data-stu-id="ee716-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="ee716-105">Para corrigir o problema, Confira estas configurações:</span><span class="sxs-lookup"><span data-stu-id="ee716-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="ee716-106">Verificar a configuração do firewall com as informações nas [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="ee716-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="ee716-107">Se o erro for específico para o proteção do Exchange Online (EOP), você deverá ter sido notificado anteriormente sobre uma alteração nos [endereços IP do Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ee716-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="ee716-108">Verifique se o seu provedor de serviços de Internet (ISP) não está bloqueando a porta.</span><span class="sxs-lookup"><span data-stu-id="ee716-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="ee716-109">Verifique as configurações de host inteligente e servidor de destino em seus conectores.</span><span class="sxs-lookup"><span data-stu-id="ee716-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="ee716-110">Observe que o Office 365 não bloqueia conexões de *entrada* dessa maneira.</span><span class="sxs-lookup"><span data-stu-id="ee716-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
