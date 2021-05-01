---
title: Problemas com o Microsoft Office SharePoint Online em máquinas Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066984"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemas com o Microsoft Office SharePoint Online em máquinas Windows 7

Se você receber erros em máquinas com Windows 7 ao trabalhar no Microsoft Office SharePoint Online ou Microsoft OneDrive, eles podem estar relacionados à suspensão do uso do TLS 1.0/1.1. Para mais informações, confira:

- [Preparando-se para TLS 1.2 no Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Os clientes Windows 7 SP1/Windows 8 devem ter o TLS1.2 habilitado. Para obter mais informações, confira [Erros de autenticação ocorrem quando o cliente não tem suporte para TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Instale o KB3140245 e crie o valor do registro. Para obter mais informações, confira  [Atualizar para habilitar TLS 1.1 e TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Os clientes Windows 7 SP1/Windows 8 devem garantir que os pacotes de criptografia TLS mais recentes sejam instalados. Para obter mais informações, confira o [Comunicado de Segurança da Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


