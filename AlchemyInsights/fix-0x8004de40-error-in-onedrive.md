---
title: Corrigir 0x8004de40 erro no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649736"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="0e7e9-102">Corrigir 0x8004de40 erro no OneDrive</span><span class="sxs-lookup"><span data-stu-id="0e7e9-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="0e7e9-103">Se você estiver executando o Windows 7 e receber esse erro, atualize para habilitar [o TLS 1.1 e o TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)como protocolos seguros padrão no WinHTTP no Windows .</span><span class="sxs-lookup"><span data-stu-id="0e7e9-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="0e7e9-104">Se você estiver executando o Windows 10 e receber um erro 0x8004de40 com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="0e7e9-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="0e7e9-105">Reboot the affected computer while connected to your Acitve Directory domain.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="0e7e9-106">Se uma reinicialização não corrigir o problema, desaja e reapresente seu dispositivo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="0e7e9-107">**Observação**: você deve estar em sua rede corporativa durante a execução dessas etapas.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="0e7e9-108">Não execute essas etapas quando você não estiver conectado à infraestrutura corporativa (por exemplo, durante a viagem).</span><span class="sxs-lookup"><span data-stu-id="0e7e9-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="0e7e9-109">Abra um prompt de comando com privilégios elevados selecionando **Iniciar**, clique com o botão direito do mouse em Prompt de **Comando** e selecione Executar **como administrador**.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="0e7e9-110">Digite *dsregcmd /leave e* pressione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="0e7e9-111">Quando estiver concluído, digite *dsregcmd /join e* pressione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="0e7e9-112">Quando estiver concluído, feche o prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="0e7e9-113">Reinicie o computador e faça logoff no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0e7e9-113">Reboot the computer, and log into OneDrive.</span></span>