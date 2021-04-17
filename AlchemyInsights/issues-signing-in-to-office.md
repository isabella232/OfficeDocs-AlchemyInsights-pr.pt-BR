---
title: Problemas ao entrar em aplicativos do Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833019"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tela de login em branco em aplicativos do Microsoft 365

Para corrigir esse problema, tente o seguinte:
- Instale as atualizações mais recentes para [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Redefinir opções do Internet Explorer: Vá para Ferramentas Opções da Internet Redefinir Configurações avançadas do Internet Explorer (observe que você perderá configurações  >    >    >  **personalizadas)** e tente entrar no Office novamente.
- Desabilite o Windows Defender do Application Guard (WDAG) ou qualquer firewall ou programa antivírus semelhante:
    1. No Painel de Controle, vá para **Programas** e, em seguida, escolha Ativar ou desativar recursos **do Windows.**
    2. Se Windows Defender o Application Guard estiver habilitado, tente desabilitá-lo.<br/>
    **Observação:** Talvez seja necessário reiniciar o computador.
- Verifique se o [plug-in WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) do Microsoft.AAD.BrokerPlugin AAD não está sendo bloqueado por nenhum aplicativo ou programa de firewall/antivírus.
- [Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.<br/>
    **Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para o [Build 16.0.7967 do Office 2016 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).