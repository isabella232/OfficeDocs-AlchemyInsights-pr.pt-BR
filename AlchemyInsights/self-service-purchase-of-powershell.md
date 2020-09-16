---
title: Compra de autoatendimento do PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739958"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="8fd5f-102">Compra de autoatendimento do PowerShell</span><span class="sxs-lookup"><span data-stu-id="8fd5f-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="8fd5f-103">Para usar o módulo MSCommerce do PowerShell, você precisa instalá-lo em um dispositivo Windows 10 com TLS 1,2 (permissões de administrador local obrigatórias).</span><span class="sxs-lookup"><span data-stu-id="8fd5f-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="8fd5f-104">Importe e conecte-se ao módulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="8fd5f-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="8fd5f-105">Quando solicitado a fazer logon, você precisará usar credenciais de função de administrador global ou de cobrança.</span><span class="sxs-lookup"><span data-stu-id="8fd5f-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="8fd5f-106">Se você não tiver o TLS 1,2, você pode receber o seguinte erro ao tentar obter ou atualizar a política:</span><span class="sxs-lookup"><span data-stu-id="8fd5f-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="8fd5f-107">*ErrorMessage-a conexão subjacente foi fechada: ocorreu um erro inesperado em um envio*.</span><span class="sxs-lookup"><span data-stu-id="8fd5f-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



