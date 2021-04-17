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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832991"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="38263-102">Corrigir os aplicativos do Microsoft 365 mensagem "O módulo plataforma confiável do seu computador não está funcionando corretamente"</span><span class="sxs-lookup"><span data-stu-id="38263-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="38263-103">Para corrigir esse erro, use as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="38263-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="38263-104">Instale as atualizações mais recentes para [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="38263-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="38263-105">[Limpar credenciais do Office usando](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) o Gerenciador de Credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="38263-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="38263-106">**Observação:** Os caminhos do Registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="38263-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="38263-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="38263-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="38263-108">Experimente o [processo de recuperação do usuário](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas do Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="38263-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="38263-109">Defina EnableADAL = 0 usando as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="38263-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="38263-110">Clique com o botão direito do mouse no botão Iniciar do Windows, escolha **Executar**, digite **regedit** e escolha **OK**.</span><span class="sxs-lookup"><span data-stu-id="38263-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="38263-111">Selecione **Sim** para permitir que o Editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38263-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="38263-112">No Editor do Registro, adicione um valor DWORD de **EnableADAL** com uma configuração **de 0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="38263-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="38263-113">Para obter mais informações, consulte Problemas de conexão na conexão após a atualização para o [Build 16.0.7967 do Office 2016 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="38263-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>