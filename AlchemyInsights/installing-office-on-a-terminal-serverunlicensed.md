---
title: Instalando o Office em um Terminal Server-não licenciado
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663105"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="54a98-102">Instalando o Office em um Terminal Server</span><span class="sxs-lookup"><span data-stu-id="54a98-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="54a98-103">Para implantar o Microsoft 365 aplicativos para empresas em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:</span><span class="sxs-lookup"><span data-stu-id="54a98-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="54a98-104">Você deve ter uma assinatura do Microsoft 365 que inclui aplicativos da Microsoft 365 para empresas, como o Office 365 Enterprise E3 ou Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="54a98-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="54a98-105">Os planos Microsoft 365 Apps for Business e Microsoft 365 aplicativos para Business Premium não incluem o Microsoft 365 aplicativos para empresas.</span><span class="sxs-lookup"><span data-stu-id="54a98-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="54a98-106">Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="54a98-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="54a98-107">Se você deseja instalar o Microsoft 365 aplicativos para empresas no RDS do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="54a98-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="54a98-108">Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Microsoft 365 aplicativos para empresas no modo de ativação de computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="54a98-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="54a98-109">Verifique a assinatura do Microsoft 365 que você tem.</span><span class="sxs-lookup"><span data-stu-id="54a98-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="54a98-110">Saiba como</span><span class="sxs-lookup"><span data-stu-id="54a98-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="54a98-111">Se necessário, alterne para uma assinatura do Microsoft 365 diferente.</span><span class="sxs-lookup"><span data-stu-id="54a98-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="54a98-112">Saiba como</span><span class="sxs-lookup"><span data-stu-id="54a98-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="54a98-113">Se o Office já estiver instalado no servidor RDS usando qualquer outra assinatura do Microsoft 365, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="54a98-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="54a98-114">Por exemplo, indo para o painel de controle \> desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="54a98-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="54a98-115">Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.</span><span class="sxs-lookup"><span data-stu-id="54a98-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="54a98-116">No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Microsoft 365 aplicativos para empresas](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="54a98-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="54a98-117">Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.</span><span class="sxs-lookup"><span data-stu-id="54a98-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="54a98-118">No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="54a98-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="54a98-119">Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar.</span><span class="sxs-lookup"><span data-stu-id="54a98-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="54a98-120">Na caixa abrir, digite **regedit**e, em seguida, selecione OK.</span><span class="sxs-lookup"><span data-stu-id="54a98-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="54a98-121">Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54a98-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="54a98-122">No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="54a98-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="54a98-123">No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Microsoft 365 aplicativos para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="54a98-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="54a98-124">Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [implantar o Microsoft 365 Apps for Enterprise usando serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="54a98-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="54a98-125">Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="54a98-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  