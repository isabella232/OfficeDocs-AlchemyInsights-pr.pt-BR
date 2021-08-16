---
title: S/MIME no Outlook na Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010712"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografar mensagens de email Outlook

Microsoft 365 A Criptografia de Mensagens é Microsoft Azure Gerenciamento de Direitos (Azure RMS), que faz parte da Proteção de Informações do Azure. Se sua assinatura incluir o Azure Rights Management ou a Proteção de Informações do Azure, não será necessário realizar nenhuma ação para habilitar ou ativar **manualmente** o Serviço de Gerenciamento de Direitos.

Com base nos comentários do cliente, não permitiremos mais que Exchange de fluxo de emails criptografe automaticamente emails de saída que contenham determinado tipo de informações confidenciais em seu locatário por padrão. Em vez disso, estamos fornecendo instruções detalhadas sobre como fazer isso sozinhos. Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte [este artigo](https://aka.ms/OmeEtr).

- Se usar Outlook na Web (anteriormente **OWA):** ao compor uma mensagem de email, clique em **Proteger** no OWA. Isso aplicará a permissão "Não encaminhar". Clique **em Alterar permissão** e escolha **Criptografar** para criptografar somente a mensagem.

- Se estiver usando **Outlook cliente**: para enviar uma mensagem criptografada do Outlook 2013 ou 2016 ou Outlook 2016 para Mac, selecione **Permissões** de Opções e selecione a opção de proteção de que  >  você precisa.

- Para **criptografar automaticamente todos** os emails enviados para determinados destinatários ou organizações de parceiros externos, você precisa criar uma regra de transporte de fluxo de emails no Centro de administração Exchange de email. Instruções detalhadas são fornecidas [neste artigo de suporte.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

