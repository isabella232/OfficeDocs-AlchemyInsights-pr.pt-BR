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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579853"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="6ff2b-102">Corrigindo os aplicativos do Microsoft 365 "a mensagem o módulo de plataforma confiável do seu computador não está funcionando adequadamente"</span><span class="sxs-lookup"><span data-stu-id="6ff2b-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="6ff2b-103">Para corrigir esse erro, use as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="6ff2b-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="6ff2b-104">Instale as atualizações mais recentes do [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [do Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6ff2b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6ff2b-105">[Limpe as credenciais do Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="6ff2b-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6ff2b-106">**Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="6ff2b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6ff2b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6ff2b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6ff2b-108">Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas no Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="6ff2b-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="6ff2b-109">Defina o EnableADAL = 0 usando as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="6ff2b-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="6ff2b-110">Clique com o botão direito do mouse no botão Iniciar do Windows, escolha **executar**, digite **regedit**e, em seguida, escolha **OK**.</span><span class="sxs-lookup"><span data-stu-id="6ff2b-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="6ff2b-111">Selecione **Sim** para permitir que o editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ff2b-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="6ff2b-112">No editor do registro, adicione um valor DWORD de **EnableADAL** com uma configuração de **0** em HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="6ff2b-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="6ff2b-113">Para obter mais informações, consulte [problemas de conexão na entrada após a atualização para o Office 2016 Build 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6ff2b-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>