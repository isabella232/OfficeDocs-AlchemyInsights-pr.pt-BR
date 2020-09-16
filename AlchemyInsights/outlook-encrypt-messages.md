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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772250"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="8abce-102">Criptografar mensagens de email no Outlook</span><span class="sxs-lookup"><span data-stu-id="8abce-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="8abce-103">A criptografia de mensagem do Microsoft 365 foi criada no Microsoft Azure Rights Management (Azure RMS), que faz parte da proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="8abce-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="8abce-104">Se sua assinatura incluir o Azure Rights Management ou o Azure Information Protection, **não será necessário realizar ações para habilitar ou desabilitar manualmente** o serviço de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="8abce-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="8abce-105">Com base nos comentários dos clientes, não ficaremos mais permitindo que as regras de fluxo de emails do Exchange criptografem automaticamente o email de saída contendo certos tipos de informações confidenciais em seu locatário por padrão.</span><span class="sxs-lookup"><span data-stu-id="8abce-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="8abce-106">Em vez disso, forneceremos instruções detalhadas sobre como você pode fazer isso yourselves.</span><span class="sxs-lookup"><span data-stu-id="8abce-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="8abce-107">Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte [Este artigo](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="8abce-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="8abce-108">Se estiver usando o Outlook na Web (anteriormente **owa**): ao redigir uma mensagem de email, basta clicar em **proteger** no OWA.</span><span class="sxs-lookup"><span data-stu-id="8abce-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="8abce-109">Isso aplicará a permissão "não encaminhar".</span><span class="sxs-lookup"><span data-stu-id="8abce-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="8abce-110">Clique em **Alterar permissão** e escolha **criptografar** para apenas criptografar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="8abce-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="8abce-111">Se estiver usando o **cliente do Outlook**: para enviar uma mensagem criptografada do Outlook 2013 ou 2016, ou do Outlook 2016 para Mac, selecione permissões de **Opções**  >  **Permissions**e, em seguida, selecione a opção de proteção de que você precisa.</span><span class="sxs-lookup"><span data-stu-id="8abce-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="8abce-112">Para **criptografar automaticamente todos os emails** enviados para determinados destinatários ou organizações de parceiros externos, você precisa criar uma regra de transporte de fluxo de emails no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8abce-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="8abce-113">As instruções detalhadas são fornecidas neste [artigo de suporte](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="8abce-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

