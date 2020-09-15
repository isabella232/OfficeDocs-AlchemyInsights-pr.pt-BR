---
title: Notificações no Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662781"
---
# <a name="notifications-in-yammer"></a>Notificações no Yammer

Para alertar você sobre novas atividades em conversas relevantes, [o Yammer envia notificações](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) por email ou, se você usa o Yammer no seu dispositivo móvel, por meio de notificações por push. Por padrão, o Yammer envia notificações para muitos tipos de atividades na sua rede. Os usuários podem atualizar suas configurações de email no site do Yammer, e as notificações por push são definidas pelo aplicativo móvel. 

O Yammer adicionou suporte para [emails interativos no Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Alguns emails (cópias de mensagem) se tornarão interativos no Outlook na Web. Uma atualização futura trará isso para outras versões do Outlook.

**Tipos de notificações no Yammer**

- Emails (atualizações de um grupo, alguém convida você para um grupo, você recebe uma mensagem na sua caixa de entrada, etc.)
- Notificações por push (enviadas para dispositivos móveis quando você é mencionado, recebe uma mensagem em sua caixa de entrada, etc.)
- Pop-ups da área de trabalho (quando o aplicativo Yammer para Área de Trabalho estiver instalado, ele exibirá notificações para os usuários, chamadas de notificações do sistema.)
- Notificações de sino (no site do Yammer, os usuários verão notificações para diferentes eventos. Essas notificações nem sempre têm um email ou uma notificação por push associados.)

[Informações mais detalhadas sobre as notificações](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) estão disponíveis.

**Gerenciar notificações**

Os usuários devem gerenciar suas próprias notificações. Informações sobre [como ativar e desativar as notificações móveis e por email do Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) estão disponíveis. 

O administradores não podem desabilitar todas as notificações ou controlar as notificações em nome dos usuários. Os administradores podem [controlar o logotipo incluído nos emails e se os usuários precisam confirmar as mensagens](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) postadas por email.

**Notificações por email enviadas para muitos usuários em sua organização**

Às vezes, uma única notificação por email será enviada pelo Yammer e recebida por muito mais usuários em sua organização do que o esperado. Isso acontece quando uma lista de distribuição ou outro tipo de endereço de email não individual são adicionados ao Yammer. O Yammer nem sempre sabe se um endereço de email pertence a um único usuário ou se é um endereço de email que fará com que um email seja entregue a muitos destinatários. Quando esse problema ocorre, você deve executar uma ação para [suspender (desativar) o usuário inválido com esse endereço de email](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) no Yammer. 

Para reduzir a chance de esse problema ocorrer, você deve:

1. [Impor a identidade do Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) para o Yammer.
2. Impedir que remetentes externos enviem emails para sua organização, ou limitar remetentes a uma lista aprovada.

Se esse problema ocorrer:

1. Identifique o destinatário do email, que deve corresponder ao usuário no Yammer. Por exemplo, all-in-sales@fabrikam.com é uma DL (lista de distribuição) para todo o pessoal de vendas. Essa DL seria identificável a partir do email do Yammer recebido pelos usuários.
2. Use o recurso [desativar (suspender) em Administração de Rede](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) para suspender o usuário que possui o endereço de e-mail all-in-sales@fabrikam.com. A suspensão pode ser desfeita; portanto, é mais segura que a exclusão. A exclusão do usuário ocorrerá automaticamente após 90 dias.
3. Opcionalmente, revise a [Exportação de Usuário](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) para identificar outros endereços de email que não sejam de usuários e que devam ser suspensos.
