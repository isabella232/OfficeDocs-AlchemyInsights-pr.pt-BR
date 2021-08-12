---
title: Enviar uma mensagem de email fornecendo a ID da mensagem de rede
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929905"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Enviar uma mensagem de email fornecendo a ID da mensagem de rede

1. No **sub-sub-sub-texto** Novo envio, selecione **Email** e **ID da Mensagem de Rede.**
2. Siga estas etapas para encontrar a ID da mensagem para uma mensagem de email Outlook:
    1. Clique duas vezes na mensagem de email para abri-la.
    1. Selecione **Propriedades de**  >  **Arquivo**.
    1. Abra Bloco de notas ou um documento do Word em branco e, em seguida, copie e colar o conteúdo encontrado na caixa **de headers** da Internet no documento aberto para melhor visibilidade.
    1. Localize **o campo X-MS-Exchange-Organization-Network-Message-Id.** O valor após **:** é a ID de que você precisa para o envio.
3. Em **Destinatários**, se o email tiver desembarcado na pasta lixo eletrônico para todos os destinatários deste email, escolha **Selecionar Todos**. Caso não seja, selecione apenas o usuário que relatou o problema.
4. Em **Motivo para envio**, se você selecionar **Deve** ter sido bloqueado , especifique se a mensagem deve ter sido bloqueada como **Spam,** **Phishing** ou **Malware** e selecione **Enviar**.

Para saber mais, confira [Como enviar spam, phishing, URLs e](https://go.microsoft.com/fwlink/?linkid=2101479)arquivos suspeitos para a Microsoft para verificação .
