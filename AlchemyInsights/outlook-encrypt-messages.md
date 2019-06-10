---
title: S/MIME no Outlook na Web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/1/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7401aa0b6e6f4cfc12290d10e3eed75a0051827b
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770949"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografar mensagens de email no Outlook

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">A criptografia de mensagem do Office 365 é criada no Microsoft Azure Rights Management (Azure RMS), que faz parte da proteção de informações do Azure. Se sua assinatura incluir o Azure Rights Management ou o Azure Information Protection, <strong style="mso-bidi-font-weight: normal;">não será necessário realizar ações para habilitar ou desabilitar manualmente</strong> o serviço de gerenciamento de direitos.</span></p> <p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Com base nos comentários dos clientes, não ficaremos mais permitindo que as regras de fluxo de emails do Exchange criptografem automaticamente o email de saída contendo certos tipos de informações confidenciais em seu locatário por padrão. &nbsp; Em vez disso, forneceremos instruções detalhadas sobre como você pode fazer isso yourselves. &nbsp;Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte este <a href="https://aka.ms/OmeEtr">artigo</a>.</span><u></u><span style="text-decoration: line-through;"></span></p> <ul> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: Symbol; mso-fareast-font-family: Symbol; mso-bidi-font-family: Symbol;"><span style="mso-list: Ignore;">&nbsp;Se &nbsp; usando o Outlook na Web (anteriormente OWA): ao redigir uma mensagem de email, basta clicar em proteger no OWA. &nbsp; &nbsp; </span> </span> <span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"> <strong style="mso-bidi-font-weight: normal;"></strong> <strong></strong> Isso se aplicará, &lsquo;por padrão,&rsquo; não encaminhará a permissão. Clique em <strong>Alterar permissão</strong> e escolha <strong>criptografar</strong> para apenas criptografar a mensagem.</span></li> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;Se estiver usando o <strong style="mso-bidi-font-weight: normal;">cliente do Outlook</strong>: para enviar uma mensagem criptografada do Outlook 2013 ou 2016, ou do Outlook 2016 &agrave; para Mac, selecione permissões de opções e, em seguida, selecione a opção de proteção de que você precisa. &nbsp; &nbsp;</span></li> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;&nbsp; Para <strong style="mso-bidi-font-weight: normal;">criptografar automaticamente todos os emails</strong> enviados para determinados destinatários ou organizações de parceiros externos, você precisa criar uma regra de transporte de fluxo de emails no centro de administração do Exchange. Instruções detalhadas são fornecidas neste <span style="color: black;"><a href="https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities">artigo de suporte</a></span></span></li> </ul>

