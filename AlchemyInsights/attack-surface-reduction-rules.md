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
# <a name="attack-surface-reduction-rules"></a>Regras de redução de superfície de ataque

A exclusão de arquivos ou pastas pode reduzir drasticamente a proteção fornecida pelas regras de redução da superfície de ataque. Os arquivos que seriam bloqueados por uma regra podem ser executados e nenhum relatório ou evento é registrado. Uma exclusão se aplica a todas as regras que permitem exclusões.

As exclusões ASR usam a mesma sintaxe que as exclusões do Microsoft Defender Antivírus. Para obter detalhes, consulte [Configurar e validar exclusões para verificações do Microsoft Defender Antivírus](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Para evitar problemas, análise [Erros comuns a evitar ao definir exclusões](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Nem todas as regras ASR suportam exclusões. Para validar se sua regra oferece suporte a exclusões, confira a tabela [Regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regras de redução de superfície de ataque

A superfície de ataque da sua organização inclui todos os locais onde um invasor pode comprometer os dispositivos ou redes da organização. Reduzir a superfície de ataque significa proteger os dispositivos e a rede da organização, o que deixa os invasores com menos maneiras de realizar ataques. A configuração das regras de redução da superfície de ataque no Microsoft Defender para Ponto de Extremidade pode ajudar.

Para mais informações, confira:

- [Mapear a regra ASR GUID para nomear](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Requisitos das regras ASR:
    - [Windows 10 Pro, versão 1709 ou posterior](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versão 1709 ou posterior](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versão 1803 (canal semestral) ou posterior](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificar a exclusão correta a ser aplicada

1. Procure eventID 1121 ou 1122 no Microsoft-Windows-Windows Defender/Log operacional.

1. Avalie o cenário de bloqueio e contexto e confirme se este cenário precisa ser desbloqueado.

1. Leia o valor do caminho nos detalhes do evento, que é o valor que define a exclusão.
    - Faça a exclusão o mais estrita possível.
    - Aplique um caractere curinga onde necessário (por exemplo, substitua a variável de Usuário).

1. Aplique a exclusão de acordo com suas necessidades de implantação. Para obter detalhes, confira [Personalizar regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>A exclusão não é honrada

1. Determine se a regra oferece suporte a exclusões. Para obter detalhes, confira [Regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Análise as exclusões aplicadas e verifique os dados do evento quanto a erros de digitação ou caracteres curinga interpretados incorretamente. Para obter mais informações, confira [ Tipos de exclusão suportados ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. se o impacto da regra for muito alto, considere mover a regra (de volta) para o modo de auditoria para realizar uma validação adicional. Para obter detalhes, confira [Testar como os recursos do Microsoft Defender para Ponto de Extremidade funcionam no modo de auditoria](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Colete dados de suporte para abrir um caso de suporte usando este comando:
    
   ** MDEClientAnalyzer.cmd -v**

    Para obter mais informações, confira [Problemas com máquinas integradas ao Microsoft Defender para Ponto de Extremidade ](issues-with-onboarding-machines.md).
