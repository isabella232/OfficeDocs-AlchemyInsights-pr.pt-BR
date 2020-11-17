---
title: Criar um grupo
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086201"
---
# <a name="create-a-group"></a><span data-ttu-id="46481-102">Criar um grupo</span><span class="sxs-lookup"><span data-stu-id="46481-102">Create a group</span></span>

<span data-ttu-id="46481-103">Este tópico descreve a criação de grupos.</span><span class="sxs-lookup"><span data-stu-id="46481-103">This topic describes group creation.</span></span>

<span data-ttu-id="46481-104">**Permissão para criar um grupo**</span><span class="sxs-lookup"><span data-stu-id="46481-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="46481-105">Certifique-se de que você está autorizado a criar um novo grupo.</span><span class="sxs-lookup"><span data-stu-id="46481-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="46481-106">Os administradores globais podem desabilitar a criação de grupos no portal do Azure ou no painel de acesso.</span><span class="sxs-lookup"><span data-stu-id="46481-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="46481-107">Você pode precisar de um administrador para criar o novo grupo ou fornecer as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="46481-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="46481-108">**Gerenciar permissões de criação de grupo**</span><span class="sxs-lookup"><span data-stu-id="46481-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="46481-109">Os administradores globais podem gerenciar permissões de criação de grupos (por motivos relacionados à segurança) ou grupos do Office 365 criados no portal do Azure ou no painel de acesso, escolhendo "os usuários podem criar grupos de segurança nos portais do Azure" ou "os usuários podem criar grupos do Office 365 no Azure Portals" em **todos os grupos**  >  **gerais (configurações)**.</span><span class="sxs-lookup"><span data-stu-id="46481-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="46481-110">Você também pode restringir a criação de grupo para selecionar um grupo de usuários se você tiver uma licença do Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="46481-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="46481-111">**Desabilitando a notificação de boas-vindas para os novos membros do grupo do Office 365**</span><span class="sxs-lookup"><span data-stu-id="46481-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="46481-112">A notificação de boas-vindas enviada aos usuários adicionados aos grupos do Office 365 pode ser desabilitada definindo **UnifiedGroupWelcomeMessageEnabled** como false no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="46481-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="46481-113">Saiba mais sobre essa configuração [aqui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="46481-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

