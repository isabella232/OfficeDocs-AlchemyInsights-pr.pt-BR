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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832991"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigir os aplicativos do Microsoft 365 mensagem "O módulo plataforma confiável do seu computador não está funcionando corretamente"

Para corrigir esse erro, use as etapas a seguir:

- Instale as atualizações mais recentes para [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.<br/>
    **Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas do Trusted Platform Module (TPM).
- Defina EnableADAL = 0 usando as seguintes etapas:  
    1. Clique com o botão direito do mouse no botão Iniciar do Windows, escolha **Executar**, digite **regedit** e escolha **OK**.
    2. Selecione **Sim** para permitir que o Editor do Registro faça alterações em seu dispositivo.
    3. No Editor do Registro, adicione um valor DWORD de **EnableADAL** com uma configuração **de 0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para o [Build 16.0.7967 do Office 2016 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).