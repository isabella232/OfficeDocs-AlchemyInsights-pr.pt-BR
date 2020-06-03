---
title: S/MIME no Outlook na Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511496"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografar mensagens de email no Outlook

A criptografia de mensagem do Microsoft 365 foi criada no Microsoft Azure Rights Management (Azure RMS), que faz parte da proteção de informações do Azure. Se sua assinatura incluir o Azure Rights Management ou o Azure Information Protection, **não será necessário realizar ações para habilitar ou desabilitar manualmente** o serviço de gerenciamento de direitos.

Com base nos comentários dos clientes, não ficaremos mais permitindo que as regras de fluxo de emails do Exchange criptografem automaticamente o email de saída contendo certos tipos de informações confidenciais em seu locatário por padrão. Em vez disso, forneceremos instruções detalhadas sobre como você pode fazer isso yourselves. Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte [Este artigo](https://aka.ms/OmeEtr).

- Se estiver usando o Outlook na Web (anteriormente **owa**): ao redigir uma mensagem de email, basta clicar em **proteger** no OWA. Isso aplicará a permissão "não encaminhar". Clique em **Alterar permissão** e escolha **criptografar** para apenas criptografar a mensagem.

- Se estiver usando o **cliente do Outlook**: para enviar uma mensagem criptografada do Outlook 2013 ou 2016, ou do Outlook 2016 para Mac, selecione permissões de **Opções**  >  **Permissions**e, em seguida, selecione a opção de proteção de que você precisa.

- Para **criptografar automaticamente todos os emails** enviados para determinados destinatários ou organizações de parceiros externos, você precisa criar uma regra de transporte de fluxo de emails no centro de administração do Exchange. As instruções detalhadas são fornecidas neste [artigo de suporte](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

