---
title: Problemas para entrar nos aplicativos do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938128"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigindo os aplicativos do Office "a mensagem o módulo de plataforma confiável do seu computador não está funcionando corretamente"

Para corrigir esse erro, tente o seguinte:

- Instale as atualizações mais recentes do [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [do Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Limpe as credenciais do Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br/>
    **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas no Trusted Platform Module (TPM).
- Defina o EnableADAL = 0 usando as seguintes etapas:  
    1. Clique com o botão direito do mouse no botão Iniciar do Windows, escolha **executar**, digite **regedit**e, em seguida, escolha **OK**.
    2. Selecione **Sim** para permitir que o editor do Registro faça alterações em seu dispositivo.
    3. No editor do registro, adicione um valor DWORD de **EnableADAL** com uma configuração de **0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obter mais informações, consulte [problemas de conexão na entrada após a atualização para o Office 2016 Build 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).