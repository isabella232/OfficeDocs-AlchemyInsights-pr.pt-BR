---
title: Corrigindo os aplicativos do Office sua conta está em uma mensagem de estado inválida
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969209"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Correção de aplicativos do Office "sua conta está em um estado inválido"

Para corrigir esse erro, tente as seguintes opções no computador afetado:

- Abra um aplicativo do Office, **** > selecione a**conta** > **de arquivo sair de todas as contas**. Entre novamente usando uma conta de usuário com uma licença válida. Para obter informações detalhadas, consulte [contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br>
  **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- No computador afetado, defina EnableADAL = 0 usando as seguintes etapas:  
     1. Clique com o botão direito do mouse no botão Windows e selecione **executar**. Na caixa **abrir** , digite **regedit**e, em seguida, selecione **OK**.
     2. Selecione **Sim** quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.
    3. No editor do registro, adicione um valor DWORD de EnableADAL com uma configuração de 0 em HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Se o erro ocorrer durante a conexão com o Office 365 usando o Office 2013, [habilite a autenticação moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.

Para obter mais informações, consulte [como solucionar problemas de aplicativos que não são do navegador que não podem entrar no Office 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

