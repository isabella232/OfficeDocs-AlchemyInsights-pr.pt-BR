---
title: Solução de problemas do Microsoft Defender para Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545256"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="7c8cc-102">Solução de problemas do Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="7c8cc-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="7c8cc-103">**Você nota atrasos na entrega de mensagens?**</span><span class="sxs-lookup"><span data-stu-id="7c8cc-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="7c8cc-104">Use a [opção Entrega Dinâmica](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) no Microsoft Defender para Office 365 Cofre De anexos.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="7c8cc-105">Isso ajudará a evitar atrasos de mensagens ao proteger destinatários de arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="7c8cc-106">**Deseja relatar falsos positivos ou falsos negativos à Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="7c8cc-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="7c8cc-107">Use [o Explorador de Envios.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="7c8cc-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="7c8cc-108">-\*\* Você sabia que pode habilitar a proteção de links Cofre para emails internos enviados entre destinatários em sua organização?\*\* Siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="7c8cc-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="7c8cc-109">Acesse e [https://protection.office.com](https://protection.office.com) entre com uma conta de administrador global ou administrador de segurança.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="7c8cc-110">No painel de navegação esquerdo em **Gerenciamento de ameaças,** escolha **Política** \> **Cofre Links.**</span><span class="sxs-lookup"><span data-stu-id="7c8cc-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="7c8cc-111">Na seção **Políticas que se aplicam a toda a organização,** selecione a política e clique em **Editar**.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="7c8cc-112">Em **Configurações**, habilita **aplicar links seguros a mensagens enviadas dentro da organização**.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
