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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="dd99f-102">Corrigir mensagens que estão presas na mensagem de saída</span><span class="sxs-lookup"><span data-stu-id="dd99f-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="dd99f-103">Recomendamos que você comece executando o cenário ["Estou tendo problemas para enviar, receber ou localizar mensagens de email"](https://aka.ms/SaRA-OutlookSendReceive) da ferramenta de [Assistente de recuperação e suporte da Microsoft](https://diagnostics.office.com/#/) na máquina afetada.</span><span class="sxs-lookup"><span data-stu-id="dd99f-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="dd99f-104">Quando uma mensagem é presa na sua mensagem de saída, a causa mais provável é um anexo grande ou a opção "enviar imediatamente quando conectado" não está habilitada.</span><span class="sxs-lookup"><span data-stu-id="dd99f-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="dd99f-105">**Remover o anexo grande**</span><span class="sxs-lookup"><span data-stu-id="dd99f-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="dd99f-106">Clique em **Enviar/receber** > **trabalho offline**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="dd99f-107">No painel de navegação, clique em **saída**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="dd99f-108">A partir daqui, você pode:</span><span class="sxs-lookup"><span data-stu-id="dd99f-108">From here, you can:</span></span> 
    - <span data-ttu-id="dd99f-109">Exclua a mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd99f-109">Delete the message.</span></span> <span data-ttu-id="dd99f-110">Basta selecioná-lo e clicar em **excluir**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="dd99f-111">Arraste a mensagem para a **pasta Rascunhos**, clique duas vezes para abrir a mensagem e exclua o anexo (clique nele e clique em **excluir**).</span><span class="sxs-lookup"><span data-stu-id="dd99f-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="dd99f-112">Se um erro informar que o Outlook está tentando transmitir a mensagem, feche o Outlook.</span><span class="sxs-lookup"><span data-stu-id="dd99f-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="dd99f-113">Pode levar alguns momentos para sair.</span><span class="sxs-lookup"><span data-stu-id="dd99f-113">It may take a few moments to exit.</span></span> <span data-ttu-id="dd99f-114">Se o Outlook não fechar, pressione **Ctrl + Alt + Delete** e clique em **iniciar o Gerenciador de tarefas**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="dd99f-115">No Gerenciador de tarefas, selecione a guia **processos** , role para baixo até Outlook. exe e clique em **finalizar processo**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="dd99f-116">Depois que o Outlook fechar, reinicie o Outlook e repita as etapas de 2-3.</span><span class="sxs-lookup"><span data-stu-id="dd99f-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="dd99f-117">Depois de remover o anexo, clique em **Enviar/receber** > **trabalho offline** para cancelar a seleção do botão e retomar o trabalho online.</span><span class="sxs-lookup"><span data-stu-id="dd99f-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="dd99f-118">As mensagens também ficam presas na mensagem de saída quando você clica em **Enviar**, mas você não está conectado.</span><span class="sxs-lookup"><span data-stu-id="dd99f-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="dd99f-119">Clique em **Enviar/receber** e observe o botão **trabalhar offline** .</span><span class="sxs-lookup"><span data-stu-id="dd99f-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="dd99f-120">Se for azul, você será desconectado.</span><span class="sxs-lookup"><span data-stu-id="dd99f-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="dd99f-121">Clique nele para se conectar (o botão fica branco) e clique em **enviar tudo**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="dd99f-122">**Habilitar o envio imediatamente quando conectado**</span><span class="sxs-lookup"><span data-stu-id="dd99f-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="dd99f-123">Na guia Arquivo, clique em **Opções**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="dd99f-124">Na caixa de diálogo Opções do Outlook, clique em **Avançado**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="dd99f-125">Na seção enviar e receber, clique para habilitar o **envio imediatamente quando conectado**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="dd99f-126">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="dd99f-126">Click **OK**.</span></span>
 
<span data-ttu-id="dd99f-127">Para obter detalhes completos, consulte:</span><span class="sxs-lookup"><span data-stu-id="dd99f-127">For full details, see:</span></span>
- [<span data-ttu-id="dd99f-128">Vídeo: enviar ou excluir um email preso</span><span class="sxs-lookup"><span data-stu-id="dd99f-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="dd99f-129">O email permanece na pasta de saída até que você inicie manualmente uma operação de envio/recebimento no Outlook</span><span class="sxs-lookup"><span data-stu-id="dd99f-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
