---
title: Instalando o Office em um Terminal Server-não licenciado
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410110"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="6c1f9-102">Instalando o Office em um Terminal Server</span><span class="sxs-lookup"><span data-stu-id="6c1f9-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="6c1f9-103">Para implantar o Office 365 proPlus em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:</span><span class="sxs-lookup"><span data-stu-id="6c1f9-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="6c1f9-104">Você deve ter um plano do Office 365 que inclua o Office 365 proPlus, como o Office 365 Enterprise E3 ou Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="6c1f9-105">Os planos do Office 365 Business e do Office 365 Business Premium não incluem o Office 365 proPlus.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="6c1f9-106">Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6c1f9-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="6c1f9-107">Se você deseja instalar o Office 365 proPlus no RDS do portal do Office 365, \* \* *que usa as configurações de instalação padrão* \* \*, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="6c1f9-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="6c1f9-108">Verifique quais são os planos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="6c1f9-109">Saiba como</span><span class="sxs-lookup"><span data-stu-id="6c1f9-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="6c1f9-110">Se necessário, alterne para um plano diferente do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="6c1f9-111">Saiba como</span><span class="sxs-lookup"><span data-stu-id="6c1f9-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="6c1f9-112">Se o Office já estiver instalado no servidor RDS usando qualquer outro plano do Office 365, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="6c1f9-113">Por exemplo, indo para o painel \> de controle desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="6c1f9-114">DesInstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="6c1f9-115">No servidor RDS, entre no portal do Office 365 com sua conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="6c1f9-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="6c1f9-116">Após a instalação do Office, \* \* *não abra ou entre* \* \* em qualquer aplicativo do Office.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="6c1f9-117">No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="6c1f9-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="6c1f9-118">Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="6c1f9-119">Na caixa abrir, digite **regedit**e, em seguida, selecione OK.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="6c1f9-120">Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="6c1f9-121">No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="6c1f9-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="6c1f9-122">No servidor RDS, \* \* *entrar como um usuário final* \* \* e verificar se [a ativação de computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="6c1f9-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="6c1f9-123">Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, confira [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="6c1f9-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="6c1f9-124">Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6c1f9-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

