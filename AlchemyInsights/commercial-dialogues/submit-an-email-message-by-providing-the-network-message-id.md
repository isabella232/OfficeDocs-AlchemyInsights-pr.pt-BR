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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735295"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Enviar uma mensagem de email fornecendo a ID da mensagem de rede

1. No **sub-sub-sub-texto** Novo envio, selecione **Email** e **ID da Mensagem de Rede.**
2. Siga estas etapas para encontrar a ID da mensagem para uma mensagem de email no Outlook:
    1. Clique duas vezes na mensagem de email para abri-la.
    1. Selecione **Propriedades de**  >  **Arquivo**.
    1. Abra o Bloco de Notas ou um documento do Word em branco e copie e colar o conteúdo encontrado na caixa **de headers** da Internet no documento aberto para melhor visibilidade.
    1. Localize o **campo X-MS-Exchange-Organization-Network-Message-Id.** O valor após **:** é a ID de que você precisa para o envio.
3. Em **Destinatários**, se o email tiver desembarcado na pasta lixo eletrônico para todos os destinatários deste email, escolha **Selecionar Todos**. Caso não seja, selecione apenas o usuário que relatou o problema.
4. Em **Motivo para envio**, se você selecionar **Deve** ter sido bloqueado , especifique se a mensagem deve ter sido bloqueada como **Spam,** **Phishing** ou **Malware** e selecione **Enviar**.

Para saber mais, confira [Como enviar spam, phishing, URLs e](https://go.microsoft.com/fwlink/?linkid=2101479)arquivos suspeitos para a Microsoft para verificação .
