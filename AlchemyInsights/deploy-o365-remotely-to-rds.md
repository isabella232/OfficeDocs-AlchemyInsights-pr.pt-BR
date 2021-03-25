---
title: Implantando aplicativos do Microsoft 365 para empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200661"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="4cbf5-102">Implantando aplicativos do Microsoft 365 para empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI</span><span class="sxs-lookup"><span data-stu-id="4cbf5-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="4cbf5-103">Para implantar o Microsoft 365 Apps para empresas usando o RDS (Remote Desktop Services), anteriormente chamado de Serviços de Terminal:</span><span class="sxs-lookup"><span data-stu-id="4cbf5-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="4cbf5-104">Você deve ter um plano do Microsoft 365 For Business ou um plano do Office 365 que inclua o Microsoft 365 Apps para empresas, como o Office 365 Enterprise E3 ou o Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="4cbf5-105">Os planos Microsoft 365 Apps for Business e Microsoft 365 Business Standard não incluem o Microsoft 365 Apps para empresas.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="4cbf5-106">Você deve [habilitar a ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="4cbf5-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="4cbf5-107">Você também pode baixar e executar o [Assistente de Recuperação](https://aka.ms/SaRA_OfficeSCA_M365Portal) e Suporte da Microsoft para instalar o Microsoft 365 Apps para empresas no modo de ativação de computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="4cbf5-108">Para obter mais informações sobre pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando a Ferramenta de Implantação do Office, consulte [Deploy Microsoft 365 Apps for enterprise by](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)using Remote Desktop Services .</span><span class="sxs-lookup"><span data-stu-id="4cbf5-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="4cbf5-109">Para corrigir erros relacionados à ativação de computador compartilhado:</span><span class="sxs-lookup"><span data-stu-id="4cbf5-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="4cbf5-110">Consulte [Solucionar problemas com a ativação de computador compartilhado para Aplicativos do Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="4cbf5-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="4cbf5-111">Consulte [Redefina os aplicativos Microsoft 365 do estado de ativação empresarial](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="4cbf5-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="4cbf5-112">Se você quiser instalar o Microsoft 365 Apps para empresas no RDS do centro de administração do Microsoft 365, que usa configurações de instalação padrão, use as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="4cbf5-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="4cbf5-113">Verifique qual assinatura você tem.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-113">Check what subscription you have.</span></span> <span data-ttu-id="4cbf5-114">[Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="4cbf5-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="4cbf5-115">Se necessário, alternar para uma assinatura diferente.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="4cbf5-116">[Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="4cbf5-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="4cbf5-117">Se o Office já estiver instalado no servidor RDS usando outras assinaturas da Microsoft, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="4cbf5-118">Por exemplo, indo para **Painel de Controle**  >  **Desinstalar um programa**.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="4cbf5-119">Desinstalar [usando o Suporte e](https://aka.ms/SARA-OfficeUninstall-Alchemy) o Assistente de Recuperação da Microsoft se você estiver com problemas.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="4cbf5-120">No servidor RDS, entre no Centro de administração do Microsoft 365 com sua conta de administrador e instale o [Microsoft 365 Apps para empresas.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="4cbf5-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="4cbf5-121">Depois que o Office for instalado, ***não abra*** ou entre em nenhum aplicativo do Office.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="4cbf5-122">No servidor RDS, habilita a ativação de computador compartilhado editando o Registro seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="4cbf5-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="4cbf5-123">Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="4cbf5-124">Na caixa Abrir, digite **regedit** e selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="4cbf5-125">Selecione **Sim** quando solicitado a permitir que o Editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="4cbf5-126">No Editor do Registro, adicione um valor de cadeia de caracteres **sharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="4cbf5-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="4cbf5-127">No servidor RDS, entre como usuário final e verifique se ***a*** ativação de computador compartilhado está habilitada para Aplicativos do [Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="4cbf5-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
