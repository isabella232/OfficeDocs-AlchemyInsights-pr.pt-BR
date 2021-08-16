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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020180"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Não é possível definir ou exibir a política AllowSelfServicePurchase

Ao tentar definir ou exibir a política AllowSelfServicePurchase, você recebe a seguinte mensagem de erro:

*HandleError : Falha ao recuperar a política de produto com PolicyId 'AllowSelfServicePurchase', ErrorMessage - A conexão subjacente foi fechada: Ocorreu um erro inesperado em um envio.*

Isso pode ser devido a uma versão mais antiga do TLS (Transport Layer Security). Para conectar o serviço MSCommerce, você precisa usar o TLS 1.2 ou superior.  

Experimente as etapas a seguir para habilitar/definir o protocolo TLS como 1.2, verificar e repetir.
 1. No prompt de comando do PowerShell (PS C: insira o seguinte comando para definir o \) protocolo TLS para a versão 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifique os protocolos TLS em uso, com o seguinte comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Repetir os comandos Get ou Update conforme necessário.

