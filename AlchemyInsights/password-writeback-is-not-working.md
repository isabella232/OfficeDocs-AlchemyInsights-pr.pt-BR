---
title: Writeback de senha não está funcionando
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324911"
---
# <a name="password-writeback-is-not-working"></a>Writeback de senha não está funcionando

**Estou com problemas para configurar o writeback de senha**

- O writeback de senha é um recurso premium.
- Certifique-se de entender os requisitos de licenciamento:
  - Você deve ter pelo menos uma licença atribuída em sua organização
  - **Usuários somente na nuvem** - SKU pago Office 365 (O365) ou Azure AD Basic
  - Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte Requisitos de licenciamento para redefinição de senha de [autoatendados do Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Você tem pelo menos uma conta de administrador e uma conta de usuário de teste com uma das licenças apropriadas.
- Você deve conectar o Azure AD Conexão o controle de domínio primário Emulator para que o writeback de senha funcione. Você pode configurar o Azure AD Conexão usar um Controlador de  Domínio Primário clicando com o botão direito do mouse nas propriedades do conector de sincronização do Active Directory e selecionando configurar partições **de** diretório. A partir daí, procure a **seção** configurações de conexão do controlador de domínio e marque a caixa intitulada apenas **use controladores de domínio preferencial.**
    **Observação**:Se o DC preferencial não for um emulador PDC, o Azure AD Conexão ainda alcançará o PDC para writeback de senha.
- A redefinição de senha foi configurada e habilitada em seu locatário. Para obter mais informações, consulte [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Certifique-se de que a conta de administrador que está sendo usada para habilitar o Writeback de Senha é uma conta de administrador de nuvem (criada no Azure AD e não no AD local)
- Você tem uma implantação local do AD única ou de várias florestas executando o Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 com os service packs mais recentes instalados
- Você tem a ferramenta de Conexão do Azure AD instalada e preparou seu ambiente do AD para sincronização com a nuvem. Antes de testar o writeback de senha, certifique-se de primeiro concluir uma importação completa e sincronização completa do AD e do Azure AD no Azure AD Conexão.
- Para saber mais, confira como fazer uma sincronização completa e importação [completa no Azure AD Conexão](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Estou tendo um problema com a conectividade de writeback de senha**

1. Baixar e habilitar a versão mais recente do [Azure AD Conexão](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuração de firewall: a ferramenta de Conexão do Azure AD (1.1.443 ou superior) precisará de acesso **HTTPS** de saída para:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permitir que as conexões ociosas persistam por pelo menos 2 a 3 minutos

**Ainda estou com problemas com o writeback de senha**

- Se você ainda estiver com dificuldades, tente desabilitar e reabilbilar o serviço de writeback de senha na ferramenta de Conexão do Azure AD
- Para saber mais, confira como [desabilitar e reabilitar o writeback de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
