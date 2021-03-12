---
title: Pesquisar e excluir mensagens de email em sua organização
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735434"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="e9159-102">Pesquisar e excluir mensagens de email em sua organização</span><span class="sxs-lookup"><span data-stu-id="e9159-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="e9159-103">Siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="e9159-103">Follow these steps:</span></span>

1. <span data-ttu-id="e9159-104">Se você não for um administrador global, para pesquisar mensagens, sua conta deverá ser adicionada ao grupo de funções do **Gerenciador** de Descobertas e Ou à função de gerenciamento **de Pesquisa de Conformidade.**</span><span class="sxs-lookup"><span data-stu-id="e9159-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="e9159-105">Para excluir mensagens, você precisará ingressar no grupo de função Gerenciamento da Organização **ou** na função de gerenciamento de Pesquisa **e Limpeza.**</span><span class="sxs-lookup"><span data-stu-id="e9159-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="e9159-106">As permissões para essas funções são atribuídas no centro de conformidade & [segurança.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="e9159-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="e9159-107">[Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="e9159-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="e9159-108">[Conectar-se ao PowerShell do Centro de Conformidade e Segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="e9159-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="e9159-109">Se você estiver usando o MFA, consulte estas instruções: Conectar-se ao Centro de Conformidade e Segurança & do PowerShell usando [a autenticação multifatória](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="e9159-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="e9159-110">Exclua a mensagem: execute `New-ComplianceSearchAction` o cmdlet para excluir a mensagem.</span><span class="sxs-lookup"><span data-stu-id="e9159-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="e9159-111">As mensagens excluídas são movidas para a pasta Itens Recuperáveis do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9159-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="e9159-112">Para um comando de exemplo, consulte [Etapa 3: Excluir a mensagem.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="e9159-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
