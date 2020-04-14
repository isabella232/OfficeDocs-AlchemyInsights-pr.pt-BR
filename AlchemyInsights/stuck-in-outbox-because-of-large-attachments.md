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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241240"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corrigir mensagens que estão presas na mensagem de saída

Recomendamos que você comece executando o cenário ["Estou tendo problemas para enviar, receber ou localizar mensagens de email"](https://aka.ms/SaRA-OutlookSendReceive) da ferramenta de [Assistente de recuperação e suporte da Microsoft](https://diagnostics.office.com/#/) .

Quando uma mensagem é presa na sua mensagem de saída, a causa mais provável é um anexo grande ou a opção "enviar imediatamente quando conectado" não está habilitada.

**Remover o anexo grande**

1. No Outlook, selecione **Enviar/receber** > **trabalho offline**. 
2. No painel de navegação, selecione a ação de **saída**. A partir daqui, você pode: 
    - Exclua a mensagem (selecione-a e, em seguida, selecione **excluir**).
    - Arraste a mensagem para a pasta Rascunhos, clique duas vezes para abri-la e remova o anexo e selecione-a e, em seguida, selecione **excluir**.
3. Se você receber um erro dizendo que o Outlook está tentando transmitir a mensagem, feche o Outlook. Pode levar alguns momentos para sair. Se o Outlook não fechar, pressione Ctrl + Alt + Delete e selecione **iniciar o Gerenciador de tarefas**. No Gerenciador de tarefas, selecione a guia **processos** , role para baixo até Outlook. exe e selecione **finalizar processo**.
4. Depois que o Outlook fechar, reinicie-o e repita as etapas 2 e 3. 
5. Depois de remover o anexo, clique em **Enviar/receber** > **trabalhar offline** para retomar o trabalho online. 

As mensagens também ficam presas na mensagem de saída quando você clica em **Enviar**, mas você não está conectado. Clique em **Enviar/receber** e observe o botão **trabalhar offline** . Se for azul, você será desconectado. Clique nele para se conectar (o botão fica branco) e clique em **enviar tudo**.
 
**Habilitar o envio imediatamente quando conectado**
 
1. Na guia Arquivo, clique em **Opções**.

2. Na caixa de diálogo Opções do Outlook, clique em **Avançado**.

3. Na seção enviar e receber, clique para habilitar o **envio imediatamente quando conectado**. Clique em **OK**.
 
Para obter detalhes completos, consulte:
- [Vídeo: enviar ou excluir um email preso](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [O email permanece na pasta de saída até que você inicie manualmente uma operação de envio/recebimento no Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
