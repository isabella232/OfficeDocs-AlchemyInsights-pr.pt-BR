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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833019"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="b38f0-102">Tela de login em branco em aplicativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b38f0-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="b38f0-103">Para corrigir esse problema, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="b38f0-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="b38f0-104">Instale as atualizações mais recentes para [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="b38f0-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b38f0-105">Redefinir opções do Internet Explorer: Vá para Ferramentas Opções da Internet Redefinir Configurações avançadas do Internet Explorer (observe que você perderá configurações  >    >    >  **personalizadas)** e tente entrar no Office novamente.</span><span class="sxs-lookup"><span data-stu-id="b38f0-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="b38f0-106">Desabilite o Windows Defender do Application Guard (WDAG) ou qualquer firewall ou programa antivírus semelhante:</span><span class="sxs-lookup"><span data-stu-id="b38f0-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="b38f0-107">No Painel de Controle, vá para **Programas** e, em seguida, escolha Ativar ou desativar recursos **do Windows.**</span><span class="sxs-lookup"><span data-stu-id="b38f0-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="b38f0-108">Se Windows Defender o Application Guard estiver habilitado, tente desabilitá-lo.</span><span class="sxs-lookup"><span data-stu-id="b38f0-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="b38f0-109">**Observação:** Talvez seja necessário reiniciar o computador.</span><span class="sxs-lookup"><span data-stu-id="b38f0-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="b38f0-110">Verifique se o [plug-in WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) do Microsoft.AAD.BrokerPlugin AAD não está sendo bloqueado por nenhum aplicativo ou programa de firewall/antivírus.</span><span class="sxs-lookup"><span data-stu-id="b38f0-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="b38f0-111">[Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="b38f0-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b38f0-112">**Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="b38f0-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b38f0-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b38f0-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="b38f0-114">Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para o [Build 16.0.7967 do Office 2016 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b38f0-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>