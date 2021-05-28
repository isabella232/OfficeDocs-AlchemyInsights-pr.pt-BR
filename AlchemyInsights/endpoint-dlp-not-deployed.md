---
title: O Ponto de extremidade da DLP não foi implantado no dispositivo do usuário
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694799"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>O Ponto de extremidade da DLP não foi implantado no dispositivo do usuário

Se a configuração da Prevenção contra perda de dados de Ponto de Extremidade (DLP) do ponto de extremidade não foi aplicada ao dispositivo de um usuário, confirme se você atende a estes requisitos:

- O Windows 10 x64 build 1809 ou posterior está instalado no dispositivo.
- O cliente anti-malware versão 4.18.2009.7 ou posterior está instalado.
- O dispositivo é **um** destes:
    
    - Azure Active Directory (Azure AD) ingressou
    - Ingressado no Azure AD híbrido
    - AAD registrado

- Para impor ações de política, certifique-se de que o navegador Microsoft Chromium Edge esteja instalado no dispositivo do ponto de extremidade.

Para requisitos adicionais para implantação do Ponto de extremidade da DLP, confira [Primeiros passos com a Prevenção contra perda de dados de Ponto de Extremidade](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).