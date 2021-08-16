---
title: Criptografar automaticamente Office 365 mensagens de email enviadas para determinados domínios
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082174"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Criptografar automaticamente Office 365 mensagens de email enviadas para determinados domínios

1. No centro [de Exchange de administração,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.** 
2. Clique no **ícone Novo (+)** e clique em **Aplicar Criptografia de Mensagens do Office 365 proteção** de direitos e direitos às mensagens .
3. Em **Nome**, insira um nome para a regra, como *Criptografar mensagens enviadas para contoso.com*.
4. In **Apply this rule if**, choose The recipient > domain **is**. 
5. Insira o nome do domínio, como **contoso.com**.
6. Clique no **ícone Adicionar (+)** e clique em **OK**.
7. Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**. 
8. No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**. (Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática. Mas você pode adicioná-lo!)
9. Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).
10. Clique em **Salvar**.

> [!IMPORTANT]
> Você sempre pode voltar e editar essa regra mais tarde.

Para obter mais informações sobre como criar regras para criptografia, consulte [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)