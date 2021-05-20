---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544566"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="aad3d-102">Alertar mensagens de email da política 'Phish Delivered due to tenant or user override'</span><span class="sxs-lookup"><span data-stu-id="aad3d-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="aad3d-103">Uma política de alerta padrão chamada "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span><span class="sxs-lookup"><span data-stu-id="aad3d-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="aad3d-104">Se você recebeu esse alerta, aqui estão as etapas para investigar:</span><span class="sxs-lookup"><span data-stu-id="aad3d-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="aad3d-105">Na mensagem de alerta, clique em **Exibir Alerta** para ir até a página **Alertas** no Centro de Conformidade & Segurança.</span><span class="sxs-lookup"><span data-stu-id="aad3d-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="aad3d-106">Selecione o alerta para ver a opção Exibir lista **de mensagens** ou Exibir mensagens **no Explorer**.</span><span class="sxs-lookup"><span data-stu-id="aad3d-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="aad3d-107">Ambas as opções levam você aos detalhes da mensagem, que inclui a ID da mensagem.</span><span class="sxs-lookup"><span data-stu-id="aad3d-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="aad3d-108">Observe que o link do Explorador de Ameaças filtrará automaticamente as mensagens que corresponderem aos critérios de alerta.</span><span class="sxs-lookup"><span data-stu-id="aad3d-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="aad3d-109">Talvez seja necessário ajustar o filtro de data no Explorador de Ameaças.</span><span class="sxs-lookup"><span data-stu-id="aad3d-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="aad3d-110">A mensagem de phishing foi entregue devido a uma substituição configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="aad3d-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="aad3d-111">Um remetente ou domínio permitido definido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="aad3d-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="aad3d-112">Um remetente ou domínio permitido definido pelo administrador em uma política anti-spam.</span><span class="sxs-lookup"><span data-stu-id="aad3d-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="aad3d-113">Um endereço IP permitido em uma política de filtro de conexão.</span><span class="sxs-lookup"><span data-stu-id="aad3d-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="aad3d-114">Uma regra de fluxo de emails (também conhecida como regra de transporte) configurada para permitir mensagens.</span><span class="sxs-lookup"><span data-stu-id="aad3d-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="aad3d-115">Se você acredita que a mensagem foi marcada incorretamente como phishing, use o Outlook [de](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Mensagem de Relatório para enviar amostras de mensagem para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="aad3d-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
