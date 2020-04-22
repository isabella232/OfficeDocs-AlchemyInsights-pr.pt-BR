---
title: O OneDrive for Business Web OneDrive é redirecionado para o Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722798"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirecionado para o Delve depois de clicar em OneDrive

Consulte nosso guia detalhado de [solução de problemas](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Para resolver esse problema, o administrador deve conceder aos usuários o direito de criar seu site de meus sites. Isso ocorre porque a página do OneDrive for Business é criada em meus sites.

Para conceder esse direito, siga estas etapas:

1. No centro de administração do SharePoint, clique em **perfis de usuário**.

2. Na seção **pessoas** , clique em **gerenciar permissões de usuário**.

3. Adicione usuários que exigem permissões para criar seu site de meus sites. Por padrão, essa configuração é definida como **todos exceto usuários externos**.

4. Depois de adicionar o usuário, os usuários ou o grupo, verifique se o usuário, os usuários ou o grupo adicionado está selecionado, role até a seção **permissões** e marque a caixa de seleção ao lado de **criar site pessoal (necessário para armazenamento pessoal, News Feed e conteúdo seguido)**.

5. Clique em **OK**e faça com que o usuário navegue até a página do onedrive para criar o site.
