---
title: Solucionar problemas com o Microsoft defender para Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801395"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="081a0-102">Solucionar problemas com o Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="081a0-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="081a0-103">**Observe atrasos com entrega de mensagem de email** ?</span><span class="sxs-lookup"><span data-stu-id="081a0-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="081a0-104">Tente usar a opção de entrega dinâmica para suas políticas de anexos seguros de ATP.</span><span class="sxs-lookup"><span data-stu-id="081a0-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="081a0-105">Isso evitará atrasos de entrega de mensagens de email ao proteger os destinatários de arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="081a0-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="081a0-106">**Você deseja relatar falsos positivos ou falsos negativos** ?</span><span class="sxs-lookup"><span data-stu-id="081a0-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="081a0-107">Use este link para enviar o arquivo para análise: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="081a0-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="081a0-108">**Você sabia que é possível habilitar a proteção de links de segurança ATP para emails enviados entre pessoas de sua organização** ?</span><span class="sxs-lookup"><span data-stu-id="081a0-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="081a0-109">Siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="081a0-109">Follow these steps:</span></span>
    1. <span data-ttu-id="081a0-110">Vá até https://protection.office.com e entre.</span><span class="sxs-lookup"><span data-stu-id="081a0-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="081a0-111">Vá para **Threat management**  >  **Policy**  >  **links seguros** da política de gerenciamento de ameaças.</span><span class="sxs-lookup"><span data-stu-id="081a0-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="081a0-112">Em **políticas que se aplicam a destinatários específicos** , edite (ou adicione) uma política.</span><span class="sxs-lookup"><span data-stu-id="081a0-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="081a0-113">Selecione **aplicar links seguros a mensagens enviadas dentro da organização** .</span><span class="sxs-lookup"><span data-stu-id="081a0-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="081a0-114">Salve sua política e aguarde cerca de 30 minutos para que as alterações funcionem da mesma forma através do datacenter.</span><span class="sxs-lookup"><span data-stu-id="081a0-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="081a0-115">Para obter mais ajuda com a ATP, consulte [Microsoft defender para Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="081a0-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>