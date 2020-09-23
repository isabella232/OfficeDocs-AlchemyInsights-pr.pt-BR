---
title: 726 bloquear o encaminhamento de email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219843"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="5b426-102">Bloqueando ou desbloqueando o encaminhamento de email</span><span class="sxs-lookup"><span data-stu-id="5b426-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="5b426-103">Para habilitar ou desabilitar o encaminhamento de emails para uma caixa de correio específica, confira [Configurar o encaminhamento de email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5b426-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="5b426-104">No nível do locatário, o controle de encaminhamento externo é feito usando a política antispam de saída.</span><span class="sxs-lookup"><span data-stu-id="5b426-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="5b426-105">Se ele estiver definido como desativado ou automático, ele poderá bloquear o encaminhamento de emails com o erro "550 5.7.520 acesso negado, sua organização não permitir encaminhamento externo".</span><span class="sxs-lookup"><span data-stu-id="5b426-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="5b426-106">Subsequentemente, se o encaminhamento estiver definido para ser bloqueado, esse será o erro que os usuários verão.</span><span class="sxs-lookup"><span data-stu-id="5b426-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="5b426-107">Se o encaminhamento estiver bloqueado, certifique-se de que a política está configurada para habilitar o avanço avançado externo.</span><span class="sxs-lookup"><span data-stu-id="5b426-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="5b426-108">Você pode verificar a política de filtro de spam de saída do centro de segurança e conformidade ou executando o comando Get-HostedOutboundSpamFilterPolicy | nome da FL, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="5b426-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="5b426-109">Se você quiser configurar o bloqueio de avanços, o mesmo comando informará o estado da política agora.</span><span class="sxs-lookup"><span data-stu-id="5b426-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="5b426-110">Observação: é recomendável manter o encaminhamento automático externo desabilitado na política de filtro de spam de saída padrão e habilitá-lo somente para os usuários que precisam de encaminhamento externo criando uma política personalizada para esses usuários.</span><span class="sxs-lookup"><span data-stu-id="5b426-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="5b426-111">Você pode ler mais sobre como [Configurar o encaminhamento de email externo no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5b426-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>