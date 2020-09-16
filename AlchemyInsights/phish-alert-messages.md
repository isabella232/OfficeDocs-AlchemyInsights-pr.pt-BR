---
title: 2491 mensagens de email de alerta da política "phishing entregue devido ao locatário ou substituição do usuário"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728599"
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
