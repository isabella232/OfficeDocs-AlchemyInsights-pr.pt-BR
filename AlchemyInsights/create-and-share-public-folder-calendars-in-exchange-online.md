---
title: Criar e compartilhar calendários de pasta pública no Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712639"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="34b2a-102">Criar e compartilhar calendários de pasta pública no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="34b2a-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="34b2a-103">Você pode criar um calendário na pasta pública somente no cliente da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="34b2a-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="34b2a-104">Use estas etapas para configurar os calendários de pasta pública:</span><span class="sxs-lookup"><span data-stu-id="34b2a-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="34b2a-105">Garanta que as pastas públicas sejam implantadas no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="34b2a-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="34b2a-106">Para saber mais, veja [Criar uma caixa de correio de pasta pública](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="34b2a-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="34b2a-107">Verifique se você tem as permissões de acesso necessárias para criar a pasta pública.</span><span class="sxs-lookup"><span data-stu-id="34b2a-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="34b2a-108">Para saber mais, confira [Permissões de pasta pública para o Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="34b2a-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="34b2a-109">Entre no cliente da área de trabalho do Outlook e garanta que você possa acessar a implantação da sua pasta pública.</span><span class="sxs-lookup"><span data-stu-id="34b2a-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="34b2a-110">Se estiver com problemas para acessar pastas públicas usando o cliente de área de trabalho do Outlook, confira [Os usuários do Exchange Online não conseguem se conectar às pastas públicas usando o Outlook ou o OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="34b2a-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="34b2a-111">Criar um novo tipo de calendário de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="34b2a-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="34b2a-112">Por padrão, a pasta pública é compartilhada com todos os outros usuários.</span><span class="sxs-lookup"><span data-stu-id="34b2a-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="34b2a-113">O proprietário da pasta pública pode alterar as permissões do cliente da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="34b2a-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="34b2a-114">Para saber mais, confira [Permissões de pasta pública para o Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="34b2a-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="34b2a-115">**Observação** Os calendários de pasta pública são projetados para serem usados dentro da organização e não podem ser publicados na Internet.</span><span class="sxs-lookup"><span data-stu-id="34b2a-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="34b2a-116">Use uma caixa de correio compartilhada se você pretende publicar um calendário na Internet.</span><span class="sxs-lookup"><span data-stu-id="34b2a-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>