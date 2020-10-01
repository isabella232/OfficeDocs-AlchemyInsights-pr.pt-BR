---
title: Configurar o Microsoft Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305431"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="1da98-102">Configurar o Microsoft Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="1da98-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="1da98-103">O Microsoft Endpoint DLP permite estender a capacidade de proteção e monitoramento de DLP a informações confidenciais em dispositivos com Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1da98-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="1da98-104">Depois que os dispositivos são integrados ao gerenciamento de dispositivos, você pode criar diretrizes de DLP para impor ações de proteção aos itens.</span><span class="sxs-lookup"><span data-stu-id="1da98-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="1da98-105">O Gerenciador de Atividade pode ser usado para monitorar a atividade de itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="1da98-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="1da98-106">Para mais informações, consulte [Dispositivo Integrados no gerenciamento de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="1da98-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="1da98-107">Iniciando com o Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="1da98-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="1da98-108">Verifique se você possui o licenciamento apropriado de SKU/assinaturas.</span><span class="sxs-lookup"><span data-stu-id="1da98-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="1da98-109">Para mais informações, consulte [licenciamento de SKU/assinaturas.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="1da98-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="1da98-110">Verifique as permissões exigidas para habilitar o gerenciamento de dispositivos, acessar a página de integração ou ativar/desativar o monitoramento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1da98-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="1da98-111">Para mais informações, consulte [Permissões](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="1da98-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="1da98-112">Dispositivos integrados dentro do gerenciamento de dispositivos, seguindo o procedimento de dispositivos integrados.</span><span class="sxs-lookup"><span data-stu-id="1da98-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="1da98-113">Se você não tiver a opção de Integração de Dispositivo (visualização) em Conformidade com o M365  \*\*Configurações \*\*, confirme se possui a licença e as permissões apropriadas mencionadas acima.</span><span class="sxs-lookup"><span data-stu-id="1da98-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="1da98-114">Para mais informações, consulte [Integração de Dispositivo](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="1da98-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="1da98-115">Crie diretrizes de DLP para proteger seus itens sigilosos.</span><span class="sxs-lookup"><span data-stu-id="1da98-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="1da98-116">Para mais informações, consulte [Cenários da diretriz DLP do Endpoint](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="1da98-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="1da98-117">Para obter mais informações sobre o Microsoft Endpoint DLP, consulte [Saiba mais sobre a prevenção de perda de dados do Microsoft 365 Endpoint (visualização)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="1da98-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="1da98-118">**Etapas de coleta de dados importantes, caso o suporte seja necessário:**</span><span class="sxs-lookup"><span data-stu-id="1da98-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="1da98-119">Baixe o MDATP Client Analyzer Preview do [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="1da98-119">Download MDATP Client Analyzer Preview from [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="1da98-120">Execute a ferramenta como Administrador na janela do cmd:</span><span class="sxs-lookup"><span data-stu-id="1da98-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="1da98-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="1da98-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="1da98-122">Quando solicitado "Digite o número de minutos para coletar rastreamentos:", insira o número de minutos necessários para executar o cenário</span><span class="sxs-lookup"><span data-stu-id="1da98-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="1da98-123">Nome do cenário</span><span class="sxs-lookup"><span data-stu-id="1da98-123">Run the scenario</span></span>

<span data-ttu-id="1da98-124">Colete a saída do arquivo zip a ser fornecido ao agente de suporte.</span><span class="sxs-lookup"><span data-stu-id="1da98-124">Collect the Zip file output to be given to the Support agent.</span></span>
