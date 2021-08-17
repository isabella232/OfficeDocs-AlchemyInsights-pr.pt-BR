---
title: Erro 401 Não autorizado no SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890254"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Erro 401 Não autorizado no SharePoint

Se você estiver recebendo a mensagem de erro "(401) Não autorizado" no SharePoint, talvez isso esteja relacionado à substituição do TLS 1.0/1.1. Para saber mais, confira:

- [Preparação para o TLS 1.2 no Office 365 e no Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Erros de autenticação ocorrem se o cliente não tiver suporte a TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atualizar para habilitar TLS 1.1 e TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se os usuários estão no Windows 7, verifiquem o [TLS Cipher Suites no Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).