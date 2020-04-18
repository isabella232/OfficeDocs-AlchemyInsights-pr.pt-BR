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
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547950"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Correção de aplicativos do Office "sua conta está em um estado inválido"

Para corrigir esse erro, tente as seguintes opções no computador afetado:

- Abra um aplicativo do Office, **File** > selecione a**conta** > **de arquivo sair de todas as contas**. Entre novamente usando uma conta de usuário com uma licença válida. Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br>
  **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- Se o erro ocorrer durante a conexão com o Office 365 usando o Office 2013, [habilite a autenticação moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.

Para obter mais informações, consulte [como solucionar problemas de aplicativos que não são do navegador que não podem entrar no Office 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

