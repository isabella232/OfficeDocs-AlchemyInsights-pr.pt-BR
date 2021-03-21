---
title: Proteção contra ataques de Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897397"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="41453-102">Proteção contra ataques de Backscatter</span><span class="sxs-lookup"><span data-stu-id="41453-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="41453-103">Backscatter são notificações de falha na entrega (também conhecidas como notificações de entrega ou mensagens de devolução) que você recebe para mensagens não enviadas.</span><span class="sxs-lookup"><span data-stu-id="41453-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="41453-104">Os remetentes de spam forjam (falsificam) o **De:** endereço de suas mensagens e costumam usar endereços de email reais para dar credibilidade às suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="41453-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="41453-105">Portanto, quando os remetentes de spam inevitavelmente enviam mensagens para destinatários não existentes, o servidor de email de destino é essencialmente enganado para retornar a mensagem não entregue em uma NDR para o remetente forjado no endereço **De:**.</span><span class="sxs-lookup"><span data-stu-id="41453-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="41453-106">Informações adicionais podem ser encontradas em [Backscatter no EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="41453-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="41453-107">**Habilitar a proteção contra Backscatter**</span><span class="sxs-lookup"><span data-stu-id="41453-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="41453-108">Para habilitar a proteção contra backscatter, siga o caminho abaixo.</span><span class="sxs-lookup"><span data-stu-id="41453-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="41453-109">**protection.office.com > Gerenciamento de Ameaças > Política > Antispam > Selecionar a Política de Filtro de Spam e Editar política > Propriedades de spam > Marcar como spam > backscatter de NDR > Definir como "Ativado"**</span><span class="sxs-lookup"><span data-stu-id="41453-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="41453-110">Se você acredita que uma conta foi comprometida, consulte o seguinte:</span><span class="sxs-lookup"><span data-stu-id="41453-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="41453-111">Responder a uma Conta de Email Comprometida</span><span class="sxs-lookup"><span data-stu-id="41453-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="41453-112">Remover usuários bloqueados do portal de Usuários Restritos no Office 365</span><span class="sxs-lookup"><span data-stu-id="41453-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



