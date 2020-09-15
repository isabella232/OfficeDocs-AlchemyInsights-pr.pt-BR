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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695167"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigindo os aplicativos do Microsoft 365 "a mensagem o módulo de plataforma confiável do seu computador não está funcionando adequadamente"

Para corrigir esse erro, use as etapas a seguir:

- Instale as atualizações mais recentes do [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [do Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Limpe as credenciais do Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br/>
    **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas no Trusted Platform Module (TPM).
- Defina o EnableADAL = 0 usando as seguintes etapas:  
    1. Clique com o botão direito do mouse no botão Iniciar do Windows, escolha **executar**, digite **regedit**e, em seguida, escolha **OK**.
    2. Selecione **Sim** para permitir que o editor do Registro faça alterações em seu dispositivo.
    3. No editor do registro, adicione um valor DWORD de **EnableADAL** com uma configuração de **0** em HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Para obter mais informações, consulte [problemas de conexão na entrada após a atualização para o Office 2016 Build 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).