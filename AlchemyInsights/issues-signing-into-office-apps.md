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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986879"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigindo Microsoft 365 aplicativos "O módulo plataforma confiável do computador não está funcionando corretamente" mensagem

Para corrigir esse erro, use as etapas a seguir:

- Instale as atualizações mais recentes [para](https://support.microsoft.com/help/4027667/windows-10-update) Windows e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Desem Office credenciais usando](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Observação:** Os caminhos do Registro para Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas do Trusted Platform Module (TPM).
- Defina EnableADAL = 0 usando as seguintes etapas:  
    1. Clique com o botão direito do mouse Windows botão Iniciar, escolha **Executar**, digite **regedit** e escolha **OK**.
    2. Selecione **Sim** para permitir que o Editor do Registro faça alterações em seu dispositivo.
    3. No Editor do Registro, adicione um valor DWORD de **EnableADAL** com uma configuração **de 0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para Office [build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)no Windows 10 .