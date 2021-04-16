---
title: Redirecionamentos do OneDrive web do OneDrive para o Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799977"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="3e8a5-102">Redirecionado para o Delve depois de clicar em OneDrive</span><span class="sxs-lookup"><span data-stu-id="3e8a5-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="3e8a5-103">Consulte nosso Guia detalhado [de Solução de Problemas.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="3e8a5-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="3e8a5-104">Para resolver esse problema, o administrador deve conceder aos usuários o direito de criar seu site meus sites.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="3e8a5-105">Isso porque a página do OneDrive for Business é criada em Meus Sites.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="3e8a5-106">Para conceder esse direito, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="3e8a5-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="3e8a5-107">No centro de administração do SharePoint, clique em **perfis de usuário**.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="3e8a5-108">Na seção **Pessoas,** clique em **Gerenciar Permissões de Usuário**.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="3e8a5-109">Adicione usuários que exigem permissões para criar seu site meus sites.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="3e8a5-110">Por padrão, essa configuração é definida como **Todos, exceto usuários externos.**</span><span class="sxs-lookup"><span data-stu-id="3e8a5-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="3e8a5-111">Depois de adicionar o usuário, usuários ou grupo, verifique se o usuário adicionado,  usuários ou grupo está selecionado, role até a seção permissões e selecione a caixa de seleção ao lado de Criar Site Pessoal (necessário para armazenamento **pessoal, newsfeed** e conteúdo seguido) .</span><span class="sxs-lookup"><span data-stu-id="3e8a5-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="3e8a5-112">Clique **em OK** e, em seguida, fazer com que o usuário navegue até a página do OneDrive para criar o site.</span><span class="sxs-lookup"><span data-stu-id="3e8a5-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
