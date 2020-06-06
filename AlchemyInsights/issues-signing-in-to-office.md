---
title: Problemas para entrar nos aplicativos do Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579889"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="4e016-102">Tela de entrada em branco nos aplicativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4e016-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="4e016-103">Para corrigir esse problema, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4e016-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="4e016-104">Instale as atualizações mais recentes do [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [do Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="4e016-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="4e016-105">Redefinir opções do Internet Explorer: Vá para **ferramentas**  >  **Opções da Internet**  >  **Advanced**  >  **redefinição avançada configurações do Internet Explorer** (Observe que você perderá as configurações personalizadas) e tente entrar novamente no Office.</span><span class="sxs-lookup"><span data-stu-id="4e016-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="4e016-106">Desabilite o Windows Defender Application Guard (WDAG) ou qualquer firewall semelhante ou programa antivírus:</span><span class="sxs-lookup"><span data-stu-id="4e016-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="4e016-107">No painel de controle, vá para **programas**e, em seguida, escolha **Ativar ou desativar recursos do Windows**.</span><span class="sxs-lookup"><span data-stu-id="4e016-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="4e016-108">Se o Windows Defender Application Guard estiver habilitado, tente desabilitá-lo.</span><span class="sxs-lookup"><span data-stu-id="4e016-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="4e016-109">**Observação:** Talvez seja necessário reiniciar o computador.</span><span class="sxs-lookup"><span data-stu-id="4e016-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="4e016-110">Verifique se o [plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BROKERPLUGIN AAD WAM não está sendo bloqueado por nenhum programa de aplicativo ou firewall/antivírus.</span><span class="sxs-lookup"><span data-stu-id="4e016-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="4e016-111">[Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="4e016-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="4e016-112">**Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="4e016-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4e016-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="4e016-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="4e016-114">Para obter mais informações, consulte [problemas de conexão na entrada após a atualização para o Office 2016 Build 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="4e016-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>