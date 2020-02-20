---
title: Não é possível definir ou exibir a política AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158545"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="ada58-102">Não é possível definir ou exibir a política AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="ada58-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="ada58-103">Ao tentar definir ou exibir a política AllowSelfServicePurchase, você recebe a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="ada58-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="ada58-104">*HandleError: falha ao recuperar a política de produto com PolicyId ' AllowSelfServicePurchase ', ErrorMessage-a conexão subjacente foi fechada: ocorreu um erro inesperado em um envio.*</span><span class="sxs-lookup"><span data-stu-id="ada58-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="ada58-105">Isso pode ser devido a uma versão mais antiga da Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="ada58-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="ada58-106">Para conectar o serviço MSCommerce, você precisa usar o TLS 1,2 ou superior.</span><span class="sxs-lookup"><span data-stu-id="ada58-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="ada58-107">Tente as seguintes etapas para habilitar/definir o protocolo TLS como 1,2, verifique e tente novamente.</span><span class="sxs-lookup"><span data-stu-id="ada58-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="ada58-108">No prompt de comando do PowerShell (PS C\) : Insira o comando a seguir para definir o protocolo TLS para a versão 1,2:</span><span class="sxs-lookup"><span data-stu-id="ada58-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="ada58-109">Verifique se os protocolos TLS em uso, com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="ada58-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="ada58-110">Repita os comandos Get ou Update, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="ada58-110">Retry the Get or Update commands as needed.</span></span>

