---
title: OneDrive for Business Web OneDrive redirecionamentos para Delve
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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922975"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirecionado para Delve depois de clicar em OneDrive

Consulte nosso Guia detalhado [de Solução de Problemas.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Para resolver esse problema, o administrador deve conceder aos usuários o direito de criar seu site meus sites. Isso porque a página OneDrive for Business é criada em Meus Sites.

Para conceder esse direito, siga estas etapas:

1. No centro de SharePoint de administração, clique em **perfis de usuário**.

2. Na seção **Pessoas,** clique em **Gerenciar Permissões de Usuário**.

3. Adicione usuários que exigem permissões para criar seu site meus sites. Por padrão, essa configuração é definida como **Todos, exceto usuários externos.**

4. Depois de adicionar o usuário, usuários ou grupo, verifique se o usuário adicionado,  usuários ou grupo está selecionado, role até a seção permissões e selecione a caixa de seleção ao lado de Criar Site Pessoal (necessário para armazenamento **pessoal, newsfeed** e conteúdo seguido) .

5. Clique **em OK** e, em seguida, fazer com que o usuário navegue até a página OneDrive para criar o site.
