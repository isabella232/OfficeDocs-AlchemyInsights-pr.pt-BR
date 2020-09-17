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
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812103"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="7c0c5-102">Configurar o Microsoft Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="7c0c5-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="7c0c5-103">O Microsoft Endpoint DLP permite estender a capacidade de proteção e monitoramento de DLP a informações confidenciais em dispositivos com Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="7c0c5-104">Depois que os dispositivos são integrados ao gerenciamento de dispositivos, você pode criar diretrizes de DLP para impor ações de proteção aos itens.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="7c0c5-105">O Gerenciador de Atividade pode ser usado para monitorar a atividade de itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="7c0c5-106">Para mais informações, consulte [Dispositivo Integrados no gerenciamento de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="7c0c5-107">Iniciando com o Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="7c0c5-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="7c0c5-108">Verifique se você possui o licenciamento apropriado de SKU/assinaturas.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="7c0c5-109">Para mais informações, consulte [licenciamento de SKU/assinaturas.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="7c0c5-110">Verifique as permissões exigidas para habilitar o gerenciamento de dispositivos, acessar a página de integração ou ativar/desativar o monitoramento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="7c0c5-111">Para mais informações, consulte [Permissões](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="7c0c5-112">Dispositivos integrados dentro do gerenciamento de dispositivos, seguindo o procedimento de dispositivos integrados.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="7c0c5-113">Se você não tiver a opção de Integração de Dispositivo (visualização) em Conformidade com o M365  \*\*Configurações \*\*, confirme se possui a licença e as permissões apropriadas mencionadas acima.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="7c0c5-114">Para mais informações, consulte [Integração de Dispositivo](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="7c0c5-115">Crie diretrizes de DLP para proteger seus itens sigilosos.</span><span class="sxs-lookup"><span data-stu-id="7c0c5-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="7c0c5-116">Para mais informações, consulte [Cenários da diretriz DLP do Endpoint](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="7c0c5-117">Para obter mais informações sobre o Microsoft Endpoint DLP, consulte [Saiba mais sobre a prevenção de perda de dados do Microsoft 365 Endpoint (visualização)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="7c0c5-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>