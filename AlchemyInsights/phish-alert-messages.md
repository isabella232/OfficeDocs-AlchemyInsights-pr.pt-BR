---
title: 2491 mensagens de email de alerta da política "phishing entregue devido ao locatário ou substituição do usuário"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758896"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Mensagens de email de alerta da política "phishing entregue devido ao locatário ou substituição do usuário"

Uma política de alerta padrão chamada "phishing entregue devido ao locatário ou substituição de usuário" foi distribuída aos locatários com as licenças do Office 365 ATP P1 e P2. Se você recebeu este alerta, veja a seguir as etapas para investigar:

1. Na mensagem de alerta, clique em **exibir alerta** para ir para a página **alertas** no centro de conformidade & segurança.

2. Selecione o alerta para ver a opção de **exibir a lista de mensagens** ou **Exibir mensagens no Explorer**. Ambas as opções levam você aos detalhes da mensagem, que inclui a ID da mensagem. Observe que o link do explorador de ameaças filtrará automaticamente as mensagens que correspondem aos critérios de alerta. Talvez seja necessário ajustar o filtro de data no Gerenciador de ameaças.

A mensagem de phishing foi entregue por causa de uma substituição configurada manualmente:

- Um remetente ou domínio permitido definido pelo usuário.

- Um remetente ou domínio permitido definido pelo administrador em uma política antispam.

- Um endereço IP permitido em uma política de filtro de conexão.

- Uma regra de fluxo de emails (também conhecida como regra de transporte) configurada para permitir mensagens no.

Se acreditar que a mensagem foi marcada incorretamente como Phish, use o suplemento de [mensagem de relatório](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) do Outlook para enviar amostras de mensagens à Microsoft.
