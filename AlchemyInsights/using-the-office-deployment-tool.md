---
title: Usando a ferramenta de implantação do Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726236"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="a768c-102">Usando a ferramenta de implantação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a768c-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a768c-103">Use a ferramenta de implantação do Office (ODT) para implantar versões do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a768c-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="a768c-104">A ferramenta de implantação do Office (Setup. exe) é executada a partir da linha de comando e usa um arquivo XML de configuração para determinar quais configurações serão aplicadas durante a implantação do Office.</span><span class="sxs-lookup"><span data-stu-id="a768c-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="a768c-105">Baixe a versão mais recente da ferramenta de implantação do Office no [centro de download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a768c-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="a768c-106">Use a [ferramenta de personalização do Office (OCT)](https://config.office.com) para selecionar suas preferências de implantação e criar o arquivo XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="a768c-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="a768c-107">Exporte o arquivo de configuração e coloque-o localmente na mesma pasta em que reside o setup. exe.</span><span class="sxs-lookup"><span data-stu-id="a768c-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="a768c-108">**Observação:** Problemas de instalação do Office geralmente ocorrem devido a arquivos de configuração incorretamente configurados ou malformatted.</span><span class="sxs-lookup"><span data-stu-id="a768c-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="a768c-109">Para evitar esses problemas, recomendamos que você use a ferramenta de personalização do Office para criar o arquivo de configuração.</span><span class="sxs-lookup"><span data-stu-id="a768c-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="a768c-110">Você também pode importar arquivos de configuração existentes para a ferramenta de personalização do Office.</span><span class="sxs-lookup"><span data-stu-id="a768c-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="a768c-111">Em um prompt de comando com privilégios elevados, alterne para o local em que o setup. exe reside e execute a ferramenta de implantação do Office no modo de download e especifique o arquivo de configuração que você acabou de salvar.</span><span class="sxs-lookup"><span data-stu-id="a768c-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="a768c-112">Neste exemplo, o arquivo de configuração é chamado de Configuration. xml:</span><span class="sxs-lookup"><span data-stu-id="a768c-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="a768c-113">Execute a ferramenta de implantação do Office no modo de configuração e especifique o arquivo de configuração.</span><span class="sxs-lookup"><span data-stu-id="a768c-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="a768c-114">**Observação:** Você deve executar esta etapa no computador cliente no qual você deseja instalar o Office e deve ter permissões de administrador local nesse computador.</span><span class="sxs-lookup"><span data-stu-id="a768c-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="a768c-115">Para saber mais sobre como usar a ferramenta de implantação do Office para seus aplicativos do Microsoft 365 para cenários de implantação corporativa, confira [visão geral da ferramenta de implantação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="a768c-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="a768c-116">Para obter mais detalhes sobre como usar a ferramenta de personalização do Office, consulte [visão geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="a768c-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
