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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744619"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemas ao entrar Microsoft 365 Apps

Observação: se você estiver usando uma versão mais antiga do Windows (por exemplo, Windows 7 SP1, Windows Server [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 2008 R2), use a correção fácil para habilitar o TLS 1.2 como padrão. Para obter mais informações, confira [Atualizar para habilitar o TLS 1.1 e o TLS 1.2 como os protocolos seguros padrão em WinHTTP no Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Para solucionar problemas de entrada nos aplicativos do Microsoft 365, tente as seguintes opções no computador afetado:  

- Para Windows, consulte [Recomendações sobre como resolver problemas](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) comuns de login
- Para Mac, consulte [Não é possível entrar em um Office 2016 para Mac aplicativo](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Dica** em computadores com Windows, podemos diagnosticar e corrigir automaticamente vários problemas de entrada comuns do Office para você. Baixe e execute o  **[Assistente de Suporte e Recuperação da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nossa ferramenta automatizada.

**Observação:** Não é recomendável desabilitar a Autenticação Moderna (ADAL) ou o Gerenciamento de Contas da Web (WAM) para corrigir problemas de login ou ativação. Se os erros ocorrerem ao se conectar ao Microsoft 365 usando o Office 2013, certifique-se de habilitar a autenticação moderna para Office cliente. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Para ações de solução de problemas específicas, consulte:

[Problemas de conexão na entrada após atualização para o build 16.0.7967 do Office 2016 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Você não pode entrar em sua conta organizacional, como Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Como solucionar problemas de aplicativos que não são do navegador que não podem entrar no Office 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Solicitado repetidamente para credenciais no Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)