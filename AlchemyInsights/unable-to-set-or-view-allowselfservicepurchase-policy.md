---
title: Não é possível definir ou exibir a política AllowSelfServicePurchase
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
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826079"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="a972f-102">Não é possível definir ou exibir a política AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="a972f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="a972f-103">Ao tentar definir ou exibir a política AllowSelfServicePurchase, você recebe a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="a972f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="a972f-104">*HandleError : Falha ao recuperar a política de produto com PolicyId 'AllowSelfServicePurchase', ErrorMessage - A conexão subjacente foi fechada: Ocorreu um erro inesperado em um envio.*</span><span class="sxs-lookup"><span data-stu-id="a972f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="a972f-105">Isso pode ser devido a uma versão mais antiga do TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="a972f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="a972f-106">Para conectar o serviço MSCommerce, você precisa usar o TLS 1.2 ou superior.</span><span class="sxs-lookup"><span data-stu-id="a972f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="a972f-107">Experimente as etapas a seguir para habilitar/definir o protocolo TLS como 1.2, verificar e repetir.</span><span class="sxs-lookup"><span data-stu-id="a972f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="a972f-108">No prompt de comando do PowerShell (PS C: insira o seguinte comando para definir o \) protocolo TLS para a versão 1.2:</span><span class="sxs-lookup"><span data-stu-id="a972f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="a972f-109">Verifique os protocolos TLS em uso, com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="a972f-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="a972f-110">Repetir os comandos Get ou Update conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="a972f-110">Retry the Get or Update commands as needed.</span></span>

