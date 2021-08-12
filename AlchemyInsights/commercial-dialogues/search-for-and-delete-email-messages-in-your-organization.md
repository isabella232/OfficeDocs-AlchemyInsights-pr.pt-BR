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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948871"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Pesquisar e excluir mensagens de email em sua organização

Siga estas etapas:

1. Se você não for um administrador global, para pesquisar mensagens, sua conta deverá ser adicionada ao grupo de funções do **Gerenciador** de Descobertas e Ou à função de gerenciamento **de Pesquisa de Conformidade.** Para excluir mensagens, você precisará ingressar no grupo de função Gerenciamento da Organização **ou** na função de gerenciamento de Pesquisa **e Limpeza.** As permissões para essas funções são atribuídas no centro de conformidade & [segurança.](https://protection.office.com)
2. [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem a ser excluído.
3. [Conectar-se ao PowerShell do Centro de Conformidade e Segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Se você estiver usando o MFA, consulte estas instruções: Conexão para o Centro de Conformidade e Segurança & do PowerShell usando a [autenticação multifatória](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Exclua a mensagem: execute `New-ComplianceSearchAction` o cmdlet para excluir a mensagem. As mensagens excluídas são movidas para a pasta Itens Recuperáveis do usuário. Para um comando de exemplo, consulte [Etapa 3: Excluir a mensagem.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
