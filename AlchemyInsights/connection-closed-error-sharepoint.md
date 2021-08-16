---
title: Erro a conexão subjacente foi fechada no SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044400"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Mensagem de erro "A conexão subjacente foi fechada" no SharePoint

Se você estiver recebendo a mensagem de erro "A conexão subjacente foi fechada" no SharePoint, talvez ela seja relacionada à substituição do TLS 1.0/1.1. Para saber mais, consulte estes artigos:

- [Preparação para o TLS 1.2 no Office 365 e no Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Erros de autenticação ocorrem se o cliente não tiver suporte a TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atualizar para habilitar TLS 1.1 e TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se os usuários estão no Windows 7, verifiquem o [TLS Cipher Suites no Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).