---
title: Corrigindo os aplicativos do Office sua conta está em uma mensagem de estado inválida
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969209"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="20971-102">Correção de aplicativos do Office "sua conta está em um estado inválido"</span><span class="sxs-lookup"><span data-stu-id="20971-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="20971-103">Para corrigir esse erro, tente as seguintes opções no computador afetado:</span><span class="sxs-lookup"><span data-stu-id="20971-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="20971-104">Abra um aplicativo do Office, \*\*\*\* > selecione a**conta** > **de arquivo sair de todas as contas**.</span><span class="sxs-lookup"><span data-stu-id="20971-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="20971-105">Entre novamente usando uma conta de usuário com uma licença válida.</span><span class="sxs-lookup"><span data-stu-id="20971-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="20971-106">Para obter informações detalhadas, consulte [contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="20971-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="20971-107">[Limpe as credenciais do Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando o Gerenciador de credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="20971-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="20971-108">**Observação:** Os caminhos do registro do Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="20971-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="20971-109">Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="20971-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="20971-110">No computador afetado, defina EnableADAL = 0 usando as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="20971-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="20971-111">Clique com o botão direito do mouse no botão Windows e selecione **executar**.</span><span class="sxs-lookup"><span data-stu-id="20971-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="20971-112">Na caixa **abrir** , digite **regedit**e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="20971-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="20971-113">Selecione **Sim** quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20971-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="20971-114">No editor do registro, adicione um valor DWORD de EnableADAL com uma configuração de 0 em HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="20971-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="20971-115">Se o erro ocorrer durante a conexão com o Office 365 usando o Office 2013, [habilite a autenticação moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="20971-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="20971-116">Para obter mais informações, consulte [como solucionar problemas de aplicativos que não são do navegador que não podem entrar no Office 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="20971-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

