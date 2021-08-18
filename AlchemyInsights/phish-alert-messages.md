---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316346"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertar mensagens de email da política 'Phish Delivered due to tenant or user override'

Uma política de alerta padrão chamada **Phish Delivered devido** a locatário ou substituição de usuário está disponível em organizações com o Microsoft Defender para licenças Office 365 P1 e P2. Se você recebeu esse alerta, aqui estão as etapas para investigar:

1. Na mensagem de alerta, clique em **Exibir Alerta** para acessar a página **Alertas** no portal Microsoft 365 Defender.

2. Selecione o alerta para ver a opção Exibir lista **de mensagens** ou Exibir mensagens **no Explorer**. Ambas as opções levam você aos detalhes da mensagem, que inclui a ID da mensagem. Observe que o link do Explorador de Ameaças filtrará automaticamente as mensagens que corresponderem aos critérios de alerta. Talvez seja necessário ajustar o filtro de data no Explorador de Ameaças.

A mensagem de phishing foi entregue devido a uma substituição configurada manualmente:

- Um remetente ou domínio permitido definido pelo usuário.
- Um remetente ou domínio permitido definido pelo administrador em uma política anti-spam.
- Um endereço IP permitido em uma política de filtro de conexão.
- Uma regra de fluxo de emails (também conhecida como regra de transporte) configurada para permitir mensagens.

Se você acredita que a mensagem foi marcada incorretamente como phishing, use [o envio](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) de Administrador para relatar a mensagem à Microsoft.

Os usuários podem usar o add-in Report Message ou o [add-in Report Phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) no Outlook enviar exemplos de mensagem para a Microsoft.
