---
title: 'Scanner do AIP: instalação e configuração'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821651"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="02d30-102">Scanner do AIP: instalação e configuração</span><span class="sxs-lookup"><span data-stu-id="02d30-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="02d30-103">**Para instalar o scanner do AIP, siga as diretrizes recomendadas**:</span><span class="sxs-lookup"><span data-stu-id="02d30-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="02d30-104">Se você estiver atualizando e não iniciando uma instalação do zero, certifique-se de que você seguiu as diretrizes para [atualizando o scanner de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e o cliente de rotulagem unificada, confira [atualizando o scanner de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="02d30-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="02d30-105">Verifique se você está em conformidade com todas as [Configurações de firewalls e de infraestrutura de rede](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="02d30-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="02d30-106">Verifique se as suas [políticas estão definidas](https://docs.microsoft.com/azure/information-protection/configure-policy) para rotular automaticamente ou tem um rótulo padrão na política.</span><span class="sxs-lookup"><span data-stu-id="02d30-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="02d30-107">Verifique se o tipo de arquivo relevante está configurado para rótulo/proteção conforme descrito em [Tipos de arquivo suportados pelo cliente de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="02d30-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="02d30-108">Além disso, se você quiser alterar o comportamento padrão, siga estas diretrizes: [Alterar o nível de proteção padrão dos arquivos](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="02d30-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="02d30-109">Verifique se a conta de usuário configurada para executar o serviço de scanner têm permissões para acessar todos os repositórios configurados.</span><span class="sxs-lookup"><span data-stu-id="02d30-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="02d30-110">Se você ainda tiver problemas, exporte os logs do scanner e adicione-os ao seu tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="02d30-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="02d30-111">**Exportar os logs do Scanner da Proteção de Informações do Azure**</span><span class="sxs-lookup"><span data-stu-id="02d30-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="02d30-112">Navegue até %localappdata%\Microsoft\MSIP no contexto de usuário que executa o serviço de scanner.</span><span class="sxs-lookup"><span data-stu-id="02d30-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="02d30-113">Zipar todo o conteúdo na pasta MSIP.</span><span class="sxs-lookup"><span data-stu-id="02d30-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="02d30-114">Salve os logs no local desejado e anexe-os à sua solicitação de serviço.</span><span class="sxs-lookup"><span data-stu-id="02d30-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="02d30-115">Você também pode usar [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="02d30-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="02d30-116">**Confira mais informações em**:</span><span class="sxs-lookup"><span data-stu-id="02d30-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="02d30-117">Implantação do scanner da Proteção de Informações do Azure para classificar e proteger arquivos automaticamente</span><span class="sxs-lookup"><span data-stu-id="02d30-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="02d30-118">Especificar e usar o Parâmetro de token para Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="02d30-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="02d30-119">Executar um ciclo de descoberta e exibir relatórios do scanner</span><span class="sxs-lookup"><span data-stu-id="02d30-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="02d30-120">Analisar a documentação da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="02d30-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="02d30-121">Requisitos da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="02d30-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="02d30-122">Baixar o cliente da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="02d30-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
