---
title: Erro 4C7 do Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795944"
---
# <a name="4c7-error-in-microsoft-teams"></a>erro 4C7 no Microsoft Teams

Este erro ocorre porque o Microsoft Teams requer autenticação de formulários. Ao implantar o AD FS (serviços de Federação do Active Directory), a autenticação de formulários não é habilitada para a intranet por padrão. Se a autenticação integrada do Windows falhar, você será solicitado a entrar usando a autenticação de formulários.

Para resolver esse problema, habilite a autenticação de formulários usando o snap-in do MMC (console de gerenciamento Microsoft) do AD FS no computador que tem a cópia local do Active Directory. Para fazer isso, execute estas etapas: 

1. No painel de navegação, navegue até **políticas de autenticação**.
2. Em **ações** no painel de detalhes, selecione **Editar Autenticação primária global**.
3. Na guia **intranet** , selecione **autenticação de formulários**.
4. Selecione **OK** (ou **aplicar**).