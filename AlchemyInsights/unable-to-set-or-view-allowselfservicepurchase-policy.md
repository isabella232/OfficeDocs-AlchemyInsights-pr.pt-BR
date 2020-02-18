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
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Não é possível definir ou exibir a política AllowSelfServicePurchase

Ao tentar definir ou exibir a política AllowSelfServicePurchase, você recebe a seguinte mensagem de erro:

*HandleError: falha ao recuperar a política de produto com PolicyId ' AllowSelfServicePurchase ', ErrorMessage-a conexão subjacente foi fechada: ocorreu um erro inesperado em um envio.*

Isso pode ser devido a uma versão mais antiga da Transport Layer Security (TLS). Para conectar o serviço MSCommerce, você precisa usar o TLS 1,2 ou superior.  

Tente as seguintes etapas para habilitar/definir o protocolo TLS como 1,2, verifique e tente novamente.
 1. No prompt de comando do PowerShell (PS C\) : Insira o comando a seguir para definir o protocolo TLS para a versão 1,2:

    \[NET. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12

2. Verifique se os protocolos TLS em uso, com o seguinte comando:

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Repita os comandos Get ou Update, conforme necessário.

