---
title: Correção de aplicativos do Microsoft 365 Não foi conseguindo encontrar licenças do office associadas a mensagem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816476"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="ce891-102">Corrigir a mensagem de aplicativos do Microsoft 365 "Não foi difícil encontrar licenças do office associadas"</span><span class="sxs-lookup"><span data-stu-id="ce891-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="ce891-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ce891-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ce891-104">Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para aplicativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ce891-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ce891-105">Consulte URLs e intervalos de [endereços IP do Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="ce891-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="ce891-106">Remova e [reatribua a licença do Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para o usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="ce891-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="ce891-107">Abra um aplicativo do Office [e saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente.</span><span class="sxs-lookup"><span data-stu-id="ce891-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="ce891-108">Vá para Configurações do Windows > **Contas** Email & contas e remova todas as contas de  >  trabalho, exceto a conta afetada.</span><span class="sxs-lookup"><span data-stu-id="ce891-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="ce891-109">Vá para Configurações do Windows > **Contas Acessar** trabalho ou escola e desconecte todas as contas de  >  trabalho, exceto a conta afetada.</span><span class="sxs-lookup"><span data-stu-id="ce891-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="ce891-110">Reinicie o estado de ativação do Office.</span><span class="sxs-lookup"><span data-stu-id="ce891-110">Reset the Office activation state.</span></span> <span data-ttu-id="ce891-111">[Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="ce891-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="ce891-112">[Entre usando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) a conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="ce891-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="ce891-113">Para obter soluções adicionais de solução de problemas, consulte [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="ce891-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>