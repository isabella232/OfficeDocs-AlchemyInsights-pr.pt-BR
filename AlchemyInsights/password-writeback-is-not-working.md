---
title: O Write-back de senha não está funcionando
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232649"
---
# <a name="password-writeback-is-not-working"></a>O Write-back de senha não está funcionando

**Estou com problemas para configurar o write-back de senha**

- O write-back de senha é um recurso premium.
- Certifique-se de que você compreende os requisitos de licenciamento:
  - Você deve ter pelo menos uma licença atribuída em sua organização
  - **Usuários somente na** nuvem - Qualquer SKU paga do Office 365 (O365) ou Azure AD Basic
  - Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, confira Requisitos de licenciamento para redefinição de senha de [autoatendado do Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Você tem pelo menos uma conta de administrador e uma conta de usuário de teste com uma das licenças apropriadas.
- Você deve conectar o Azure AD Connect ao Emulador controlador de domínio primário para que o write-back de senha funcione. Você pode configurar o Azure AD Connect para usar  um Controlador de Domínio Primário clicando com o botão direito do mouse nas propriedades do conector de sincronização do Active Directory e selecionando configurar partições **de diretório.** A partir daí, procure a **seção** de configurações de conexão do controlador de domínio e marque a caixa intitulo apenas para **usar controladores de domínio preferenciais.**
  > [!NOTE]
  > Se o DC preferencial não for um emulador PDC, o Azure AD Connect ainda chegará ao PDC para write-back de senha.
- A redefinição de senha foi configurada e habilitada em seu locatário. Para saber mais, confira [Habilitar os usuários a redefinir suas senhas do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Certifique-se de que a conta de administrador que está sendo usada para habilitar o Write-back de Senha seja uma conta de administrador de nuvem (criada no Azure AD e não no AD local)
- Você tem uma implantação local do AD de floresta única ou com várias florestas executando o Windows Server 2008 R2, o Windows Server 2012 ou o Windows Server 2012 R2 com os service packs mais recentes instalados
- Você tem a ferramenta Azure AD Connect instalada e preparou seu ambiente do AD para sincronização com a nuvem. Antes de testar o write-back de senha, primeiro certifique-se de concluir uma importação completa e uma sincronização completa do AD e do Azure AD no Azure AD Connect.
- Para saber mais, veja como fazer uma sincronização completa e [a importação completa no Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Estou tendo um problema com a conectividade de write-back de senha**

1. Baixar e habilitar a versão mais recente do [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuração de firewall: a ferramenta Azure AD Connect (1.1.443 e superior) precisará de acesso **HTTPS** de saída para:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permitir que conexões ociosas persistam por pelo menos 2 a 3 minutos

**Ainda estou tendo problemas com o write-back de senha**

- Se você ainda estiver com dificuldades, tente desabilitar e reabilgrafar o serviço de write-back de senha na ferramenta Azure AD Connect
- Para saber mais, veja como desabilitar [e reabilitar o write-back de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
