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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657917"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="1b996-102">Configurar o Microsoft Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="1b996-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="1b996-103">O Microsoft Endpoint DLP permite estender a capacidade de proteção e monitoramento de DLP a informações confidenciais em dispositivos com Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1b996-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="1b996-104">Depois que os dispositivos são integrados ao gerenciamento de dispositivos, você pode criar diretrizes de DLP para impor ações de proteção aos itens.</span><span class="sxs-lookup"><span data-stu-id="1b996-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="1b996-105">O Gerenciador de Atividade pode ser usado para monitorar a atividade de itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="1b996-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="1b996-106">Para mais informações, consulte [Dispositivo Integrados no gerenciamento de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="1b996-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="1b996-107">Iniciando com o Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="1b996-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="1b996-108">Verifique se você possui o licenciamento apropriado de SKU/assinaturas.</span><span class="sxs-lookup"><span data-stu-id="1b996-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="1b996-109">Para mais informações, consulte [licenciamento de SKU/assinaturas.](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="1b996-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="1b996-p103">Verifique as permissões exigidas para habilitar o gerenciamento de dispositivos, acessar a página de integração ou ativar/desativar o monitoramento de dispositivos. Para mais informações, confira [Permissões](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="1b996-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="1b996-112">Dispositivos integrados no Gerenciamento de dispositivos, seguindo o procedimento de dispositivos integrados.</span><span class="sxs-lookup"><span data-stu-id="1b996-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="1b996-113">Para mais informações, consulte [Integração de Dispositivo](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="1b996-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="1b996-114">Crie diretrizes de DLP para proteger seus itens sigilosos.</span><span class="sxs-lookup"><span data-stu-id="1b996-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="1b996-115">Para mais informações, consulte [Cenários da diretriz DLP do Endpoint](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="1b996-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="1b996-116">Para obter mais informações sobre o Microsoft Endpoint DLP, consulte [Saiba mais sobre a prevenção de perda de dados do Microsoft 365 Endpoint (visualização)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="1b996-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="1b996-117">**Etapas de coleta de dados importantes, caso o suporte seja necessário:**</span><span class="sxs-lookup"><span data-stu-id="1b996-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="1b996-118">Baixe o [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="1b996-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="1b996-119">Execute a ferramenta como Administrador na janela do cmd:</span><span class="sxs-lookup"><span data-stu-id="1b996-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="1b996-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="1b996-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="1b996-121">Quando for solicitado **Insira o número de minutos para coletar rastreamentos:**, insira o número de minutos necessários para executar o cenário.</span><span class="sxs-lookup"><span data-stu-id="1b996-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="1b996-122">Execute o cenário.</span><span class="sxs-lookup"><span data-stu-id="1b996-122">Run the scenario.</span></span>

<span data-ttu-id="1b996-123">Coletar a saída do arquivo ZIP para entregar ao agente de suporte.</span><span class="sxs-lookup"><span data-stu-id="1b996-123">Collect the Zip file output to give to the Support agent.</span></span>
