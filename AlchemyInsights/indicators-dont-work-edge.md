---
title: Os indicadores não funcionam com o navegador Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: 4094371ee0a3b3ec8d29454fd66f3e9e7c3f35a91b9ea05f308325bc447ce11c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926305"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Os indicadores não funcionam com o navegador Edge

Depois de criar um indicador, ele não é respeitado pelo Edge (Smartscreen). Para obter mais informações, confira [Criar indicadores para IPs e URLs/domínios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Etapa 1: certifique-se do seguinte

- Verifique se o indicador está correto (sem erros de digitação no IP/URL, ação correta, os grupos RBAC corretos).
- Aguarde no mínimo 2 horas após a criação do indicador para levar em consideração qualquer latência possível.
- Confirme se os sistemas estão integrados ao Microsoft Defender para Ponto de Extremidade.
- Verifique se o(s) sistema(s) podem se comunicar com a nuvem.
- Verifique se o Smartscreen está habilitado e acessível acessando o [site de teste](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Etapa 2: solucionar o problema potencial

- Certifique-se de que o cliente atende aos requisitos. Para obter detalhes, confira [Criar indicadores para IPs e URLs/domínios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Certifique-se de que está executando a versão mais recente do navegador Edge. Para descobrir a versão mais recente, confira [Descubra qual versão do Microsoft Edge você possui](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Reinicie o navegador Edge.
- Navegue até o site para o qual você configurou um indicador. Se o site não aparecer conforme o esperado, vá para a Etapa 3. 

## <a name="step-3-collect-data"></a>Etapa 3: coletar dados

- Colete dados de diagnóstico **MDEClientAnalyzer**. Para obter instruções, confira [Problemas com máquinas integradas ao Microsoft Defender para Ponto de Extremidade](issues-with-onboarding-machines.md).
- Se você se sentir confortável em instalar e coletar um rastreio do Fiddler, confira [Telerik Fiddler](http://www.telerik.com/fiddler).
- Se você preferir orientação do Suporte da Microsoft, selecione o ícone Suporte abaixo para abrir um caso de suporte.
