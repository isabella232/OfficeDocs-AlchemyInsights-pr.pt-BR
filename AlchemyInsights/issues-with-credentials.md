---
title: Problemas com credenciais
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052941"
---
# <a name="issues-with-credentials"></a>Problemas com credenciais

[A microsoft identity platform and the OAuth 2.0 client credentials flow describes](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) how to program directly against the OAuth 2.0 client credentials grant flow.

**Como faço para gerenciar a senha ou as credenciais de certificado de um aplicativo?**

Na CLI do Azure, você pode usar a credencial do aplicativo [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) para excluir, listar ou redefinir as credenciais de senha ou certificado de um aplicativo.

**Como meus usuários redefinem suas senhas?**

Os usuários precisam [se registrar para redefinir senhas](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) de autoatendados antes de redefinir suas senhas. Depois que um usuário se registrar, ele poderá seguir as instruções neste artigo para redefinir sua senha: [redefinir sua senha de](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)trabalho ou de estudante.

**Como meus usuários alteram suas senhas?**

Os usuários podem seguir as etapas deste artigo para alterar suas senhas: [Como alterar sua senha.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Eles também podem [gerenciar senhas de aplicativo para verificação em duas etapas.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Meu usuário está recebendo um erro ao alterar ou redefinir a senha**

Este link fornecerá informações sobre problemas comuns que podem surgir quando um usuário está tentando redefinir sua senha: problemas [comuns e suas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Estou com um problema para redefinir a senha de um usuário**

- Certifique-se de que você está autorizado a redefinir senhas. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.

- Certifique-se de entender os requisitos de licenciamento:

  - Você deve ter pelo menos uma licença atribuída em sua organização:
    - **Usuários somente na** nuvem - Qualquer SKU paga do Office 365 (O365) ou Azure AD Basic
    - Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, confira Requisitos de licenciamento para redefinição de senha de [autoatendado do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Para redefinir a senha de um usuário, encontre o usuário no Azure AD. Em seguida, na folha visão geral desse usuário, clique no botão "redefinir senha".

**O botão de redefinição de senha está acinzentado**

Você não está autorizado a **redefinir** as senhas desse usuário. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.

**Não vejo a folha de redefinição de senha**

Você não está autorizado a redefinir senhas. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.

**Não vejo a folha de integração local na redefinição de senha**

- A folha de integração local só aparece em ambientes híbridos, o que significa que você está usando o write-back de senha para manipular as senhas do usuário local.

- Você não verá essa folha se:

  - Você não está usando write-back de senha
  - Há um problema com a instalação/conectividade do write-back de senha
  - Há um problema com sua instalação/conectividade do Azure AD Connect
  - Para obter mais etapas de solução de problemas com o write-back de senha, consulte [Solucionar problemas de write-re de senha](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Não sei como redefinir a senha de um usuário**

1. Entre no portal do Azure como um administrador apropriado.
2. Vá até a **folha Usuários e grupos,** selecione **Todos os Usuários.**
3. Selecione um usuário na lista.
4. Para o usuário selecionado, selecione **Visão Geral** e, na barra de comandos, selecione **Redefinir senha.**
5. Selecione o **botão Redefinir** senha e siga as instruções na tela.
    - Somente redefinições realizadas por meio do **portal do Azure suportam** write-back de senha.

**Redefini a senha de um usuário local do portal de administração do Office 365 ou do aplicativo móvel do Office 365, mas o usuário ainda não consegue entrar**

O Write-back de senha não é suportado neste portal. Redefinir a senha do usuário novamente no portal do Azure.
