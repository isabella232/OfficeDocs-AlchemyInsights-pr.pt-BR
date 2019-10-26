---
title: Instalando o Office em um Terminal Server-não licenciado
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205397"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8892b-102">Instalando o Office em um Terminal Server</span><span class="sxs-lookup"><span data-stu-id="8892b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8892b-103">Para implantar o Office 365 ProPlus em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:</span><span class="sxs-lookup"><span data-stu-id="8892b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8892b-104">Você deve ter um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="8892b-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8892b-105">Os planos do Office 365 Business e do Office 365 Business Premium não incluem o Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="8892b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="8892b-106">Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8892b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="8892b-107">Se você deseja instalar o Office 365 ProPlus no RDS a partir do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="8892b-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8892b-108">Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8892b-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8892b-109">Verifique quais são os planos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8892b-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8892b-110">Saiba como</span><span class="sxs-lookup"><span data-stu-id="8892b-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8892b-111">Se necessário, alterne para um plano diferente do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8892b-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8892b-112">Saiba como</span><span class="sxs-lookup"><span data-stu-id="8892b-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8892b-113">Se o Office já estiver instalado no servidor RDS usando qualquer outro plano do Office 365, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="8892b-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8892b-114">Por exemplo, indo para o painel \> de controle desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="8892b-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8892b-115">Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.</span><span class="sxs-lookup"><span data-stu-id="8892b-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8892b-116">No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8892b-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8892b-117">Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.</span><span class="sxs-lookup"><span data-stu-id="8892b-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8892b-118">No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="8892b-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8892b-119">Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar.</span><span class="sxs-lookup"><span data-stu-id="8892b-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8892b-120">Na caixa abrir, digite **regedit**e, em seguida, selecione OK.</span><span class="sxs-lookup"><span data-stu-id="8892b-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8892b-121">Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8892b-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8892b-122">No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8892b-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8892b-123">No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8892b-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="8892b-124">Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, confira [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8892b-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8892b-125">Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8892b-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  