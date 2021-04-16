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
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirecionado para o Delve depois de clicar em OneDrive

Consulte nosso Guia detalhado [de Solução de Problemas.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Para resolver esse problema, o administrador deve conceder aos usuários o direito de criar seu site meus sites. Isso porque a página do OneDrive for Business é criada em Meus Sites.

Para conceder esse direito, siga estas etapas:

1. No centro de administração do SharePoint, clique em **perfis de usuário**.

2. Na seção **Pessoas,** clique em **Gerenciar Permissões de Usuário**.

3. Adicione usuários que exigem permissões para criar seu site meus sites. Por padrão, essa configuração é definida como **Todos, exceto usuários externos.**

4. Depois de adicionar o usuário, usuários ou grupo, verifique se o usuário adicionado,  usuários ou grupo está selecionado, role até a seção permissões e selecione a caixa de seleção ao lado de Criar Site Pessoal (necessário para armazenamento **pessoal, newsfeed** e conteúdo seguido) .

5. Clique **em OK** e, em seguida, fazer com que o usuário navegue até a página do OneDrive para criar o site.
