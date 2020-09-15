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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695311"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Correção dos aplicativos do Microsoft 365 "Desculpe, outra conta da sua organização já está conectada" "Message

Para corrigir esse erro, use as etapas a seguir:

- Remover todas as contas de trabalho, exceto a conta afetada, usando as configurações do Windows > **acessar o trabalho ou a escola**.
- [Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.<br/>
    **Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra um aplicativo do Office, escolha a conta de **arquivo**  >  **Account**  >  **sair**. Em seguida, entre usando uma conta de usuário com uma licença válida. Para informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para o Mac, consulte [Não é possível entrar em um aplicativo do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para saber mais, confira ["a outra conta da sua organização já entrou neste computador" no Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).