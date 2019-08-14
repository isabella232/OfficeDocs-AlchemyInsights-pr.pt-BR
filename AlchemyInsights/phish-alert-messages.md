---
title: 2491 mensagens de email de alerta da política "phishing entregue devido ao locatário ou substituição do usuário"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391100"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="9aeb3-102">Mensagens de email de alerta da política "phishing entregue devido ao locatário ou substituição do usuário"</span><span class="sxs-lookup"><span data-stu-id="9aeb3-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="9aeb3-103">Uma política de alerta padrão chamada "phishing entregue devido ao locatário ou substituição de usuário" foi distribuída aos locatários com as licenças do Office 365 ATP P1 e P2.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="9aeb3-104">Se você recebeu este alerta, veja a seguir as etapas para investigar:</span><span class="sxs-lookup"><span data-stu-id="9aeb3-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="9aeb3-105">Na mensagem de alerta, clique em **exibir alerta** para ir para a página **alertas** no centro de conformidade & segurança.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="9aeb3-106">Selecione o alerta para ver a opção de **exibir a lista de mensagens** ou **Exibir mensagens no Explorer**.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="9aeb3-107">Ambas as opções levam você aos detalhes da mensagem, que inclui a ID da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="9aeb3-108">Observe que o link do explorador de ameaças filtrará automaticamente as mensagens que correspondem aos critérios de alerta.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="9aeb3-109">Talvez seja necessário ajustar o filtro de data no Gerenciador de ameaças.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="9aeb3-110">A mensagem de phishing foi entregue por causa de uma substituição configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="9aeb3-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="9aeb3-111">Um remetente ou domínio permitido definido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="9aeb3-112">Um remetente ou domínio permitido definido pelo administrador em uma política antispam.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="9aeb3-113">Um endereço IP permitido em uma política de filtro de conexão.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="9aeb3-114">Uma regra de fluxo de emails (também conhecida como regra de transporte) configurada para permitir mensagens no.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="9aeb3-115">Se acreditar que a mensagem foi marcada incorretamente como Phish, use o suplemento de [mensagem de relatório](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) do Outlook para enviar amostras de mensagens à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9aeb3-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
