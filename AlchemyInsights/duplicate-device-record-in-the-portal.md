---
title: Registro de dispositivo duplicado no portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789551"
---
# <a name="duplicate-device-record-in-the-portal"></a>Registro de dispositivo duplicado no portal

Você pode ver dois registros de um dispositivo no portal se o dispositivo não relatar corretamente o status de cogerenciamento no site do Gerenciador de Configurações. Para verificar o status de cogerenciamento de um dispositivo, verifique a coluna **Cogerenciado** para o dispositivo no console do Gerenciador de Configurações. Se a coluna não estiver visível, você poderá adicioná-la clicando com o botão direito do mouse em qualquer um dos cabeçalhos da coluna e selecionando-a na lista.

O valor cogerenciado deve ser **Sim**. Se o valor for **Não**, abra o miniaplicativo de cliente do Gerenciador de Configurações no dispositivo do cliente e verifique a propriedade **Cogerenciamento** na guia Geral.

- Se o valor estiver **Habilitado**, isso indicará problemas com a comunicação do cliente com o Ponto de Gerenciamento. Verifique o **CcmMessaging.log** no dispositivo para investigar possíveis problemas de conectividade.

- Se o valor estiver **Desabilitado** e o dispositivo estiver registrado no Intune, certifique-se de que o dispositivo recebeu a política de gerenciamento de cogerenciamento verificando o** CoManagementHandler.log** no dispositivo.
