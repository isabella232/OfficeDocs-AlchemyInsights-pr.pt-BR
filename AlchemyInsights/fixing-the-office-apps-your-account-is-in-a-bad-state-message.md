---
title: Corrigindo os aplicativos Microsoft 365 sua conta está em uma mensagem de estado inválida
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744533"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Corrigindo o Microsoft 365 aplicativos "a conta está em um estado inválido"

Para corrigir esse erro, tente as seguintes opções no computador afetado:

- Abra um aplicativo do Office, **File**selecione a  >  **conta**  >  **de arquivo sair de todas as contas**. Entre novamente usando uma conta de usuário com uma licença válida. Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br>
  **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- Se o erro ocorrer durante a conexão com o Office 365 usando o Office 2013, [habilite a autenticação moderna](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.

Para obter mais informações, consulte [como solucionar problemas de aplicativos que não são do navegador que não podem entrar no Microsoft 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

