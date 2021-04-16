---
title: Compra self-service do PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797709"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="96cf1-102">Compra self-service do PowerShell</span><span class="sxs-lookup"><span data-stu-id="96cf1-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="96cf1-103">Para usar o módulo MSCommerce PowerShell, você precisa instalá-lo em um dispositivo Windows 10 com TLS 1.2 (permissões de administrador local necessárias).</span><span class="sxs-lookup"><span data-stu-id="96cf1-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="96cf1-104">Importe e conecte-se ao módulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="96cf1-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="96cf1-105">Quando solicitado a fazer logoff, você precisará usar credenciais de função administrador global ou de cobrança.</span><span class="sxs-lookup"><span data-stu-id="96cf1-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="96cf1-106">Se você não tiver o TLS 1.2, poderá receber o seguinte erro ao tentar obter ou atualizar a política:</span><span class="sxs-lookup"><span data-stu-id="96cf1-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="96cf1-107">*ErrorMessage - A conexão subjacente foi fechada: Ocorreu* um erro inesperado em um envio .</span><span class="sxs-lookup"><span data-stu-id="96cf1-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



