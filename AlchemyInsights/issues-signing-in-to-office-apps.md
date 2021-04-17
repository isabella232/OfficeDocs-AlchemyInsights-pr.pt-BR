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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833063"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corrigir os aplicativos do Microsoft 365 Mensagem "Desculpe, outra conta da sua organização já está assinada"

Para corrigir esse erro, use as etapas a seguir:

- Remova todas as contas de trabalho, exceto a conta afetada, usando Configurações do Windows > **Trabalho ou escola do Access.**
- [Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.<br/>
    **Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra um aplicativo do Office, escolha **Sair** da  >  **Conta**  >  **de Arquivo**. Em seguida, entre usando uma conta de usuário com uma licença válida. Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para o Mac, consulte [Não é possível entrar em um aplicativo do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obter mais informações, consulte ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).