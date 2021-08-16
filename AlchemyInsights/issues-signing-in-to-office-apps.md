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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028028"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corrigir os Microsoft 365 aplicativos "Desculpe, outra conta da sua organização já está assinada" mensagem

Para corrigir esse erro, use as etapas a seguir:

- Remova todas as contas de trabalho, exceto a conta afetada, usando Windows Configurações > **trabalho ou escola do Access.**
- [Desem Office credenciais usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Observação:** Os caminhos do Registro para Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra um Aplicativo do Office, escolha **Sair** da  >  **Conta de**  >  **Arquivo**. Em seguida, entre usando uma conta de usuário com uma licença válida. Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para o Mac, consulte [Não é possível entrar em um aplicativo do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obter mais informações, consulte ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).