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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="d0395-102">Corrigir mensagens que estão presas na mensagem de saída</span><span class="sxs-lookup"><span data-stu-id="d0395-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="d0395-103">Recomendamos que você comece executando o cenário ["Estou tendo problemas para enviar, receber ou localizar mensagens de email"](https://aka.ms/SaRA-OutlookSendReceive) da ferramenta de [Assistente de recuperação e suporte da Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="d0395-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="d0395-104">Quando uma mensagem é presa na sua mensagem de saída, a causa mais provável é um anexo grande ou a opção "enviar imediatamente quando conectado" não está habilitada.</span><span class="sxs-lookup"><span data-stu-id="d0395-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="d0395-105">**Remover o anexo grande**</span><span class="sxs-lookup"><span data-stu-id="d0395-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="d0395-106">No Outlook, selecione **Enviar/receber** > **trabalho offline**.</span><span class="sxs-lookup"><span data-stu-id="d0395-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="d0395-107">No painel de navegação, selecione a ação de **saída**.</span><span class="sxs-lookup"><span data-stu-id="d0395-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="d0395-108">A partir daqui, você pode:</span><span class="sxs-lookup"><span data-stu-id="d0395-108">From here, you can:</span></span> 
    - <span data-ttu-id="d0395-109">Exclua a mensagem (selecione-a e, em seguida, selecione **excluir**).</span><span class="sxs-lookup"><span data-stu-id="d0395-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="d0395-110">Arraste a mensagem para a pasta Rascunhos, clique duas vezes para abri-la e remova o anexo e selecione-a e, em seguida, selecione **excluir**.</span><span class="sxs-lookup"><span data-stu-id="d0395-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="d0395-111">Se você receber um erro dizendo que o Outlook está tentando transmitir a mensagem, feche o Outlook.</span><span class="sxs-lookup"><span data-stu-id="d0395-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="d0395-112">Pode levar alguns momentos para sair.</span><span class="sxs-lookup"><span data-stu-id="d0395-112">It may take a few moments to exit.</span></span> <span data-ttu-id="d0395-113">Se o Outlook não fechar, pressione Ctrl + Alt + Delete e selecione **iniciar o Gerenciador de tarefas**.</span><span class="sxs-lookup"><span data-stu-id="d0395-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="d0395-114">No Gerenciador de tarefas, selecione a guia **processos** , role para baixo até Outlook. exe e selecione **finalizar processo**.</span><span class="sxs-lookup"><span data-stu-id="d0395-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="d0395-115">Depois que o Outlook fechar, reinicie-o e repita as etapas 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="d0395-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="d0395-116">Depois de remover o anexo, clique em **Enviar/receber** > **trabalhar offline** para retomar o trabalho online.</span><span class="sxs-lookup"><span data-stu-id="d0395-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="d0395-117">As mensagens também ficam presas na mensagem de saída quando você clica em **Enviar**, mas você não está conectado.</span><span class="sxs-lookup"><span data-stu-id="d0395-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="d0395-118">Clique em **Enviar/receber** e observe o botão **trabalhar offline** .</span><span class="sxs-lookup"><span data-stu-id="d0395-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="d0395-119">Se for azul, você será desconectado.</span><span class="sxs-lookup"><span data-stu-id="d0395-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="d0395-120">Clique nele para se conectar (o botão fica branco) e clique em **enviar tudo**.</span><span class="sxs-lookup"><span data-stu-id="d0395-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="d0395-121">**Habilitar o envio imediatamente quando conectado**</span><span class="sxs-lookup"><span data-stu-id="d0395-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="d0395-122">Na guia Arquivo, clique em **Opções**.</span><span class="sxs-lookup"><span data-stu-id="d0395-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="d0395-123">Na caixa de diálogo Opções do Outlook, clique em **Avançado**.</span><span class="sxs-lookup"><span data-stu-id="d0395-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="d0395-124">Na seção enviar e receber, clique para habilitar o **envio imediatamente quando conectado**.</span><span class="sxs-lookup"><span data-stu-id="d0395-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="d0395-125">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0395-125">Click **OK**.</span></span>
 
<span data-ttu-id="d0395-126">Para obter detalhes completos, consulte:</span><span class="sxs-lookup"><span data-stu-id="d0395-126">For full details, see:</span></span>
- [<span data-ttu-id="d0395-127">Vídeo: enviar ou excluir um email preso</span><span class="sxs-lookup"><span data-stu-id="d0395-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="d0395-128">O email permanece na pasta de saída até que você inicie manualmente uma operação de envio/recebimento no Outlook</span><span class="sxs-lookup"><span data-stu-id="d0395-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
