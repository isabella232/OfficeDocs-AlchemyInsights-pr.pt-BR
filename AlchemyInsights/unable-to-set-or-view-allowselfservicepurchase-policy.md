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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091658"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="ef28a-102">Não é possível definir ou exibir a política AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="ef28a-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="ef28a-103">Ao tentar definir ou exibir a política AllowSelfServicePurchase, você recebe a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="ef28a-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="ef28a-104">*HandleError: falha ao recuperar a política de produto com PolicyId ' AllowSelfServicePurchase ', ErrorMessage-a conexão subjacente foi fechada: ocorreu um erro inesperado em um envio.*</span><span class="sxs-lookup"><span data-stu-id="ef28a-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="ef28a-105">Isso pode ser devido a uma versão mais antiga da Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="ef28a-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="ef28a-106">Para conectar o serviço MSCommerce, você precisa usar o TLS 1,2 ou superior.</span><span class="sxs-lookup"><span data-stu-id="ef28a-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="ef28a-107">Tente as seguintes etapas para habilitar/definir o protocolo TLS como 1,2, verifique e tente novamente.</span><span class="sxs-lookup"><span data-stu-id="ef28a-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="ef28a-108">No prompt de comando do PowerShell (PS C\) : Insira o comando a seguir para definir o protocolo TLS para a versão 1,2:</span><span class="sxs-lookup"><span data-stu-id="ef28a-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="ef28a-109">\[NET. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="ef28a-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="ef28a-110">Verifique se os protocolos TLS em uso, com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="ef28a-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="ef28a-111">\[NET. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="ef28a-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="ef28a-112">Repita os comandos Get ou Update, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="ef28a-112">Retry the Get or Update commands as needed.</span></span>

