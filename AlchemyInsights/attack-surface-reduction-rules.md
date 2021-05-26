---
title: Regras de redução de superfície de ataque
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651471"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="813b7-102">Regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="813b7-102">Attack surface reduction rules</span></span>

<span data-ttu-id="813b7-103">A exclusão de arquivos ou pastas pode reduzir drasticamente a proteção fornecida pelas regras de redução da superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="813b7-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="813b7-104">Os arquivos que seriam bloqueados por uma regra podem ser executados e nenhum relatório ou evento é registrado.</span><span class="sxs-lookup"><span data-stu-id="813b7-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="813b7-105">Uma exclusão se aplica a todas as regras que permitem exclusões.</span><span class="sxs-lookup"><span data-stu-id="813b7-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="813b7-106">As exclusões ASR usam a mesma sintaxe que as exclusões do Microsoft Defender Antivírus.</span><span class="sxs-lookup"><span data-stu-id="813b7-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="813b7-107">Para obter detalhes, consulte [Configurar e validar exclusões para verificações do Microsoft Defender Antivírus](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="813b7-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="813b7-108">Para evitar problemas, análise [Erros comuns a evitar ao definir exclusões](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="813b7-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="813b7-109">Nem todas as regras ASR suportam exclusões.</span><span class="sxs-lookup"><span data-stu-id="813b7-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="813b7-110">Para validar se sua regra oferece suporte a exclusões, confira a tabela [Regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="813b7-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="813b7-111">Regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="813b7-111">Attack surface reduction rules</span></span>

<span data-ttu-id="813b7-112">A superfície de ataque da sua organização inclui todos os locais onde um invasor pode comprometer os dispositivos ou redes da organização.</span><span class="sxs-lookup"><span data-stu-id="813b7-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="813b7-113">Reduzir a superfície de ataque significa proteger os dispositivos e a rede da organização, o que deixa os invasores com menos maneiras de realizar ataques.</span><span class="sxs-lookup"><span data-stu-id="813b7-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="813b7-114">A configuração das regras de redução da superfície de ataque no Microsoft Defender para Ponto de Extremidade pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="813b7-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="813b7-115">Para mais informações, confira:</span><span class="sxs-lookup"><span data-stu-id="813b7-115">For more information, see:</span></span>

- [<span data-ttu-id="813b7-116">Mapear a regra ASR GUID para nomear</span><span class="sxs-lookup"><span data-stu-id="813b7-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="813b7-117">Requisitos das regras ASR:</span><span class="sxs-lookup"><span data-stu-id="813b7-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="813b7-118">Windows 10 Pro, versão 1709 ou posterior</span><span class="sxs-lookup"><span data-stu-id="813b7-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="813b7-119">Windows 10 Enterprise, versão 1709 ou posterior</span><span class="sxs-lookup"><span data-stu-id="813b7-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="813b7-120">Windows Server, versão 1803 (canal semestral) ou posterior</span><span class="sxs-lookup"><span data-stu-id="813b7-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="813b7-121">Identificar a exclusão correta a ser aplicada</span><span class="sxs-lookup"><span data-stu-id="813b7-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="813b7-122">Procure eventID 1121 ou 1122 no Microsoft-Windows-Windows Defender/Log operacional.</span><span class="sxs-lookup"><span data-stu-id="813b7-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="813b7-123">Avalie o cenário de bloqueio e contexto e confirme se este cenário precisa ser desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="813b7-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="813b7-124">Leia o valor do caminho nos detalhes do evento, que é o valor que define a exclusão.</span><span class="sxs-lookup"><span data-stu-id="813b7-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="813b7-125">Faça a exclusão o mais estrita possível.</span><span class="sxs-lookup"><span data-stu-id="813b7-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="813b7-126">Aplique um caractere curinga onde necessário (por exemplo, substitua a variável de Usuário).</span><span class="sxs-lookup"><span data-stu-id="813b7-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="813b7-127">Aplique a exclusão de acordo com suas necessidades de implantação.</span><span class="sxs-lookup"><span data-stu-id="813b7-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="813b7-128">Para obter detalhes, confira [Personalizar regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="813b7-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="813b7-129">A exclusão não é honrada</span><span class="sxs-lookup"><span data-stu-id="813b7-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="813b7-130">Determine se a regra oferece suporte a exclusões.</span><span class="sxs-lookup"><span data-stu-id="813b7-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="813b7-131">Para obter detalhes, confira [Regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="813b7-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="813b7-132">Análise as exclusões aplicadas e verifique os dados do evento quanto a erros de digitação ou caracteres curinga interpretados incorretamente.</span><span class="sxs-lookup"><span data-stu-id="813b7-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="813b7-133">Para obter mais informações, confira [ Tipos de exclusão suportados ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="813b7-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="813b7-134">se o impacto da regra for muito alto, considere mover a regra (de volta) para o modo de auditoria para realizar uma validação adicional.</span><span class="sxs-lookup"><span data-stu-id="813b7-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="813b7-135">Para obter detalhes, confira [Testar como os recursos do Microsoft Defender para Ponto de Extremidade funcionam no modo de auditoria](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="813b7-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="813b7-136">Colete dados de suporte para abrir um caso de suporte usando este comando:</span><span class="sxs-lookup"><span data-stu-id="813b7-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="813b7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="813b7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="813b7-138">Para obter mais informações, confira [Problemas com máquinas integradas ao Microsoft Defender para Ponto de Extremidade ](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="813b7-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
