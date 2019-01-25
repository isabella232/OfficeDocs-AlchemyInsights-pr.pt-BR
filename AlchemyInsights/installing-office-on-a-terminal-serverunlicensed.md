---
title: Instalar o office em um servidor de Terminal - não licenciado
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457151"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="e19e9-102">Instalar o Office em um servidor de Terminal</span><span class="sxs-lookup"><span data-stu-id="e19e9-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="e19e9-103">Para implantar o Office 365 ProPlus em um servidor do Windows usando os serviços de área de trabalho remota (RDS), anteriormente conhecido como serviços de Terminal:</span><span class="sxs-lookup"><span data-stu-id="e19e9-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="e19e9-p101">Você deve ter um plano do Office 365 que inclui o Office 365 ProPlus, como o Office 365 Enterprise E3 ou E5 da empresa. Os planos de negócios do Office 365 e Office 365 Business Premium não incluem Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="e19e9-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="e19e9-106">Você precisará habilitar [a ativação do computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e19e9-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="e19e9-107">Se você deseja instalar o Office 365 ProPlus em RDS do portal do Office 365, \* \* *que usa as configurações de instalação padrão* \* \*, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="e19e9-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="e19e9-p102">Verifique que você tem de plano do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="e19e9-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="e19e9-p103">Se necessário, alternar para um diferentes do Office 365 planejar. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="e19e9-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="e19e9-p104">Se o Office já estiver instalado no servidor RDS usando outros planos do Office 365, desinstale-o. Por exemplo, indo para painel de controle \> desinstalar um programa. Desinstale o usando o [Assistente de recuperação e de suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando nestes problemas.</span><span class="sxs-lookup"><span data-stu-id="e19e9-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="e19e9-115">No servidor RDS, entre no portal do Office 365 com sua conta de administrador e [instalar o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="e19e9-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="e19e9-116">Após a instalação do Office, \* \* *não abrir ou entrar* \* \* para quaisquer aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="e19e9-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="e19e9-117">No servidor RDS, habilite ativação do computador compartilhado por meio da edição do registro, seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="e19e9-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="e19e9-p105">Com o botão direito no botão do Windows no canto inferior esquerdo da tela e selecione Executar. Na caixa Abrir, digite **regedit**e, em seguida, selecione Okey.</span><span class="sxs-lookup"><span data-stu-id="e19e9-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="e19e9-120">Selecione Sim quando solicitado para permitir que o Editor do registro para fazer alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e19e9-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="e19e9-121">No Editor do registro, adicione um valor de cadeia de caracteres do **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="e19e9-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="e19e9-122">No servidor RDS, \* \* *entrar como um usuário final* \* \* e [Verificar se a ativação do computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="e19e9-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="e19e9-123">Para obter mais detalhes sobre os pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [Implantar o Office 365 ProPlus, usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="e19e9-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="e19e9-124">Para corrigir erros relacionados à ativação do computador compartilhado, consulte [Solucionar problemas com a ativação do computador compartilhado do Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e19e9-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

