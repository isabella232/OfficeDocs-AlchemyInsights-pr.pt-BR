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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986807"
---
# <a name="issues-with-credentials"></a>Problemas com credenciais

plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrevem como programar diretamente em relação ao fluxo de concessão de credenciais do cliente OAuth 2.0.

**Como gerenciar a senha ou as credenciais de certificado de um aplicativo?**

Na CLI do Azure, você pode usar a credencial do [aplicativo do az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) para excluir, listar ou redefinir as credenciais de senha ou certificado de um aplicativo.

**Como meus usuários redefinem suas senhas?**

Os usuários precisam se [registrar para redefinir a](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) senha de autoatendados antes de redefinir suas senhas. Depois que um usuário se registrou, ele pode seguir as instruções neste artigo para redefinir sua senha: Redefinir sua senha de [trabalho ou de estudante.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Como meus usuários alteram suas senhas?**

Os usuários podem seguir as etapas deste artigo para alterar suas senhas: [Como alterar sua senha](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Eles também podem [Gerenciar senhas de aplicativo para verificação em duas etapas.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Meu usuário está recebendo um erro ao alterar ou redefinir a senha**

Este link fornecerá informações sobre problemas comuns que podem surgir quando um usuário está tentando redefinir sua senha: [problemas comuns e suas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Estou com problemas para redefinir a senha de um usuário**

- Certifique-se de que você está autorizado a redefinir senhas. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.

- Certifique-se de entender os requisitos de licenciamento:

  - Você deve ter pelo menos uma licença atribuída em sua organização:
    - **Usuários somente na nuvem** - SKU pago Office 365 (O365) ou Azure AD Basic
    - Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte Requisitos de licenciamento para redefinição de senha de [autoatendados do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Para redefinir a senha de um usuário, encontre o usuário no Azure AD. Em seguida, na folha de visão geral desse usuário, clique no botão "redefinir senha".

**O botão de redefinição de senha está acinzentado**

Você não está autorizado a **redefinir** as senhas desse usuário. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.

**Não vejo a folha de redefinição de senha**

Você não está autorizado a redefinir senhas. *Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.* Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.

**Não vejo a folha de integração local na redefinição de senha**

- A folha de integração local só aparece em ambientes híbridos , o que significa que você está usando o writeback de senha para manipular as senhas do usuário local.

- Você não verá essa folha se:

  - Você não está usando writeback de senha
  - Há um problema com a instalação/conectividade do writeback de senha
  - Há um problema com sua instalação/conectividade do Azure AD Conexão
  - Para obter mais etapas de solução de problemas para problemas com o writeback de senha, consulte [Solucionar problemas de writeback de senha](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Não sei como redefinir a senha de um usuário**

1. Entre no portal do Azure como um administrador apropriado.
2. Vá para a **folha Usuários e grupos,** selecione **Todos os Usuários**.
3. Selecione um usuário na lista.
4. Para o usuário selecionado, selecione **Visão Geral** e, em seguida, na barra de comandos, selecione **Redefinir senha**.
5. Selecione o **botão Redefinir senha** e siga as instruções na tela.
    - Somente as redefinições realizadas por meio do **portal do Azure** suportam o writeback de senha.

**Redefini a senha de um usuário local do portal de administração Office 365 ou do aplicativo móvel Office 365, mas o usuário ainda não consegue entrar**

O Writeback de senha não é suportado neste portal. Redefinir a senha do usuário novamente no portal do Azure.
