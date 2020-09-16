---
title: Corrigindo aplicativos do Microsoft 365 não foi possível encontrar a mensagem associada ao Office licenses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747683"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="86f1a-102">Corrigindo a mensagem "o Microsoft 365 aplicativos" não foi possível encontrar licenças do Office associadas "</span><span class="sxs-lookup"><span data-stu-id="86f1a-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="86f1a-103">Se você receber essa mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="86f1a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="86f1a-104">Verifique as configurações de firewall, software antivírus e proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="86f1a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="86f1a-105">Consulte [URLs e intervalos de endereços IP do Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="86f1a-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="86f1a-106">Remova e [reatribua a licença do Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para o usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="86f1a-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="86f1a-107">Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente.</span><span class="sxs-lookup"><span data-stu-id="86f1a-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="86f1a-108">Vá para configurações do Windows > **contas**  >  de**email & contas**e remova todas as contas de trabalho, exceto a conta afetada.</span><span class="sxs-lookup"><span data-stu-id="86f1a-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="86f1a-109">Vá para configurações do Windows > acessar **contas**de  >  **trabalho ou escola**e desconectar todas as contas de trabalho, exceto a conta afetada.</span><span class="sxs-lookup"><span data-stu-id="86f1a-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="86f1a-110">Reinicie o estado de ativação do Office.</span><span class="sxs-lookup"><span data-stu-id="86f1a-110">Reset the Office activation state.</span></span> <span data-ttu-id="86f1a-111">[Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="86f1a-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="86f1a-112">[Entre](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="86f1a-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="86f1a-113">Para soluções de solução de problemas adicionais, confira o artigo não [licenciado e erros de ativação no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="86f1a-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>