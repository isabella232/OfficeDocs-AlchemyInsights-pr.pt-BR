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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="7b433-102">Problemas com o Microsoft Office SharePoint Online em máquinas Windows 7</span><span class="sxs-lookup"><span data-stu-id="7b433-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="7b433-103">Se você receber erros em máquinas com Windows 7 ao trabalhar no Microsoft Office SharePoint Online ou Microsoft OneDrive, eles podem estar relacionados à suspensão do uso do TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="7b433-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="7b433-104">Para mais informações, confira:</span><span class="sxs-lookup"><span data-stu-id="7b433-104">For more information, see:</span></span>

- [<span data-ttu-id="7b433-105">Preparando-se para TLS 1.2 no Office 365 e Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="7b433-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="7b433-106">Os clientes Windows 7 SP1/Windows 8 devem ter o TLS1.2 habilitado.</span><span class="sxs-lookup"><span data-stu-id="7b433-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="7b433-107">Para obter mais informações, confira [Erros de autenticação ocorrem quando o cliente não tem suporte para TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="7b433-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="7b433-108">Instale o KB3140245 e crie o valor do registro.</span><span class="sxs-lookup"><span data-stu-id="7b433-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="7b433-109">Para obter mais informações, confira  [Atualizar para habilitar TLS 1.1 e TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="7b433-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="7b433-110">Os clientes Windows 7 SP1/Windows 8 devem garantir que os pacotes de criptografia TLS mais recentes sejam instalados.</span><span class="sxs-lookup"><span data-stu-id="7b433-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="7b433-111">Para obter mais informações, confira o [Comunicado de Segurança da Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="7b433-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


