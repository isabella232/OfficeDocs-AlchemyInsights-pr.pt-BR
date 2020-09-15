---
title: Criar um relacionamento de organização para permitir que seus usuários colabore em outra organização
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712721"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="f4a0d-102">Criar um relacionamento de organização para permitir que seus usuários colabore em outra organização</span><span class="sxs-lookup"><span data-stu-id="f4a0d-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="f4a0d-103">No painel do Centro de administração do Microsoft 365, acesse **Administrador** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="f4a0d-104">Ir para **compartilhamento** > **da organização**.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="f4a0d-105">Em **Compartilhamento de Organização**, clique em **Novo**.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="f4a0d-106">Em **novo relacionamento de organização**, na caixa **Nome do relacionamento**, digite um nome amigável para o relacionamento de organização.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="f4a0d-107">Na caixa **Domínios com os quais compartilhar**, digite o domínio para o Office 365 externo ou a organização local do Exchange que você deseja permitir que vejam seus calendários.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="f4a0d-108">Se quiser inserir mais de um domínio, separe os nomes de domínio com vírgulas.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="f4a0d-109">Por exemplo, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="f4a0d-p102">Desmarque a caixa de seleção **Habilitar compartilhamento de informações de disponibilidade de calendário** para ativar o compartilhamento de calendário com os domínios listados. Defina o nível de compartilhamento para as informações de disponibilidade de calendário e defina quais usuários poderão compartilhar informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="f4a0d-112">Para definir o nível de disponibilidade de acesso, selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="f4a0d-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="f4a0d-113">**Informações de disponibilidade do calendário somente com as horas**</span><span class="sxs-lookup"><span data-stu-id="f4a0d-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="f4a0d-114">**Disponibilidade de calendário com hora, assunto e local**</span><span class="sxs-lookup"><span data-stu-id="f4a0d-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="f4a0d-115">Para definir quais usuários internos compartilharão as informações de disponibilidade de calendário, selecione uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="f4a0d-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="f4a0d-116">**Todos em sua organização**</span><span class="sxs-lookup"><span data-stu-id="f4a0d-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="f4a0d-117">**Um grupo de segurança especificado**</span><span class="sxs-lookup"><span data-stu-id="f4a0d-117">**A specified security group**</span></span>  

<span data-ttu-id="f4a0d-118">Clique em **procurar** para selecionar o grupo de segurança em uma lista, e clique em **ok**.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="f4a0d-119">Clique em **salvar** para criar o relacionamento da organização.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="f4a0d-120">**Observação:** configurações de locatários cruzados não oferecem suporte a contatos pessoais para pesquisa de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="f4a0d-121">Os contatos devem ser incluídos na lista de endereços global para a pesquisa de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4a0d-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="f4a0d-122">**Para obter o conhecimento completo deste tópico, leia:**</span><span class="sxs-lookup"><span data-stu-id="f4a0d-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="f4a0d-123">Criar um relacionamento de organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f4a0d-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="f4a0d-124">Modificar um relacionamento de organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f4a0d-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="f4a0d-125">Remover um relacionamento de organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f4a0d-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
