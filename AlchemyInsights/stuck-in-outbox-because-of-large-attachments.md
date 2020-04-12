---
title: Preso na saída por causa de anexos grandes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232618"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corrigir mensagens que estão presas na mensagem de saída

Recomendamos que você comece executando o cenário ["Estou tendo problemas para enviar, receber ou localizar mensagens de email"](https://aka.ms/SaRA-OutlookSendReceive) da ferramenta de [Assistente de recuperação e suporte da Microsoft](https://diagnostics.office.com/#/) na máquina afetada.

Quando uma mensagem é presa na sua mensagem de saída, a causa mais provável é um anexo grande ou a opção "enviar imediatamente quando conectado" não está habilitada.

**Remover o anexo grande**

1. Clique em **Enviar/receber** > **trabalho offline**. 
2. No painel de navegação, clique em **saída**. A partir daqui, você pode: 
    - Exclua a mensagem. Basta selecioná-lo e clicar em **excluir**.
    - Arraste a mensagem para a **pasta Rascunhos**, clique duas vezes para abrir a mensagem e exclua o anexo (clique nele e clique em **excluir**).
3. Se um erro informar que o Outlook está tentando transmitir a mensagem, feche o Outlook. Pode levar alguns momentos para sair. Se o Outlook não fechar, pressione **Ctrl + Alt + Delete** e clique em **iniciar o Gerenciador de tarefas**. No Gerenciador de tarefas, selecione a guia **processos** , role para baixo até Outlook. exe e clique em **finalizar processo**.
4. Depois que o Outlook fechar, reinicie o Outlook e repita as etapas de 2-3. 
5. Depois de remover o anexo, clique em **Enviar/receber** > **trabalho offline** para cancelar a seleção do botão e retomar o trabalho online. 

As mensagens também ficam presas na mensagem de saída quando você clica em **Enviar**, mas você não está conectado. Clique em **Enviar/receber** e observe o botão **trabalhar offline** . Se for azul, você será desconectado. Clique nele para se conectar (o botão fica branco) e clique em **enviar tudo**.
 
**Habilitar o envio imediatamente quando conectado**
 
1. Na guia Arquivo, clique em **Opções**.

2. Na caixa de diálogo Opções do Outlook, clique em **Avançado**.

3. Na seção enviar e receber, clique para habilitar o **envio imediatamente quando conectado**. Clique em **OK**.
 
Para obter detalhes completos, consulte:
- [Vídeo: enviar ou excluir um email preso](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [O email permanece na pasta de saída até que você inicie manualmente uma operação de envio/recebimento no Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
