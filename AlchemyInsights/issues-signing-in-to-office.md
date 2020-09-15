---
title: Problemas para entrar nos aplicativos do Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695275"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tela de entrada em branco nos aplicativos do Microsoft 365

Para corrigir esse problema, tente o seguinte:
- Instale as atualizações mais recentes do [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [do Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Redefinir opções do Internet Explorer: Vá para **ferramentas**  >  **Opções da Internet**  >  **Advanced**  >  **redefinição avançada configurações do Internet Explorer** (Observe que você perderá as configurações personalizadas) e tente entrar novamente no Office.
- Desabilite o Windows Defender Application Guard (WDAG) ou qualquer firewall semelhante ou programa antivírus:
    1. No painel de controle, vá para **programas**e, em seguida, escolha **Ativar ou desativar recursos do Windows**.
    2. Se o Windows Defender Application Guard estiver habilitado, tente desabilitá-lo.<br/>
    **Observação:** Talvez seja necessário reiniciar o computador.
- Verifique se o [plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BROKERPLUGIN AAD WAM não está sendo bloqueado por nenhum programa de aplicativo ou firewall/antivírus.
- [Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br/>
    **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obter mais informações, consulte [problemas de conexão na entrada após a atualização para o Office 2016 Build 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).