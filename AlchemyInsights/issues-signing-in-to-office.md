---
title: Problemas ao entrar em Microsoft 365 aplicativos
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
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088024"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tela de login em branco em Microsoft 365 aplicativos

Para corrigir esse problema, tente o seguinte:
- Instale as atualizações mais recentes [para](https://support.microsoft.com/help/4027667/windows-10-update) Windows e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Redefinir opções do Internet Explorer: Vá para Ferramentas Opções da Internet Redefinir o Internet Explorer avançado Configurações (observe que você perderá configurações  >    >    >   personalizadas) e tente entrar no Office novamente.
- Desabilite o Windows Defender Application Guard (WDAG) ou qualquer firewall ou programa antivírus semelhante:
    1. No Painel de Controle, vá para **Programas** e, em seguida, escolha Ativar ou desativar Windows **recursos.**
    2. Se Windows Defender Application Guard estiver habilitado, tente desabilitá-lo.<br/>
    **Observação:** Talvez seja necessário reiniciar o computador.
- Verifique se o [plug-in WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) do Microsoft.AAD.BrokerPlugin AAD não está sendo bloqueado por nenhum aplicativo ou programa de firewall/antivírus.
- [Desem Office credenciais usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Observação:** Os caminhos do Registro para Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para Office [build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)no Windows 10 .