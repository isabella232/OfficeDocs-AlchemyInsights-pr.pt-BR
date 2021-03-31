---
title: EndPoint Manager - Linhas de base de segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440862"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="bf968-102">EndPoint Manager - Linhas de base de segurança</span><span class="sxs-lookup"><span data-stu-id="bf968-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="bf968-103">As linhas de base de segurança são grupos pré-configurados de configurações do Windows que ajudam você a aplicar as configurações de segurança recomendadas pelas equipes de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="bf968-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="bf968-104">Essas linhas de base podem ser personalizadas para entregar apenas as configurações e valores desejados.</span><span class="sxs-lookup"><span data-stu-id="bf968-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="bf968-105">Para mais informações sobre linhas de base de segurança, consulte [Utilizar linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="bf968-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="bf968-106">Existem atualmente linhas de base para esses produtos:</span><span class="sxs-lookup"><span data-stu-id="bf968-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="bf968-107">Configurações de segurança do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="bf968-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="bf968-108">Segurança do Microsoft Defender para Ponto de Extremidade</span><span class="sxs-lookup"><span data-stu-id="bf968-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="bf968-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bf968-109">Microsoft Edge</span></span>

<span data-ttu-id="bf968-110">Cada uma das linhas de base são atualizadas periodicamente e lançadas em versões incrementais.</span><span class="sxs-lookup"><span data-stu-id="bf968-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="bf968-111">Cada versão adiciona e remove as configurações da versão anterior para garantir que a linha de base atenda às orientações atuais.</span><span class="sxs-lookup"><span data-stu-id="bf968-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="bf968-112">O console de linhas de base de Segurança na Segurança do Ponto de extremidade permite que diferentes versões sejam comparadas, tornando visíveis as mudanças de versão para versão.</span><span class="sxs-lookup"><span data-stu-id="bf968-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="bf968-113">Para orientações sobre como alterar, com mais eficácia, qual versão da linha de base será implantada, consulte [Gerenciar perfis de linha de base de segurança no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="bf968-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="bf968-114">Após a implantação de uma linha de base de segurança, você pode monitorar o estado da implantação e analisar as configurações com base em cada dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf968-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="bf968-115">**Observação:** Os dados de relatórios para linhas de base podem levar até 24 horas para aparecer a partir da implantação inicial para um dispositivo e até 6 horas para novas atualizações.</span><span class="sxs-lookup"><span data-stu-id="bf968-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="bf968-116">A causa mais comum da não aplicação de uma configuração de base é porque a mesma configuração está sendo utilizada em um perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="bf968-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="bf968-117">Este cenário pode ser investigado para um dispositivo específico, selecionando esse dispositivo dentro do nó de Status do Dispositivo do perfil da Linha de Base de Segurança.</span><span class="sxs-lookup"><span data-stu-id="bf968-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="bf968-118">Para maiores detalhes, consulte [Resolver conflitos para linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="bf968-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>