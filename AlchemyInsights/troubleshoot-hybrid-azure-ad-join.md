---
title: Ingresso no Azure AD híbrido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939259"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Ingresso no Azure AD híbrido

Altamente recomendado Certifique-se de que um dispositivo pode acessar is pontos de extremidade do Registro de Dispositivo na conta do sistema usando o [Script de Teste de Conectividade de Registro de Dispositivo](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Se você estiver configurando os registros de dispositivos pela primeira vez, certifique-se de revisar a [Introdução ao gerenciamento de dispositivos no Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) para saber como colocar os dispositivos sob o controle do Azure AD.
1. Se você estiver registrando diretamente os dispositivos no Azure Active Directory e inscrevendo-os no Intune, certifique-se de ter [configurado o Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o [licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) em vigor primeiro.
1. Verifique se você está autorizado a executar operações no Azure Active Directory e no AD local. Apenas um administrador global no Azure Active Directory pode gerenciar as configurações para registros de dispositivos. Além disso, se estiver configurando os registros automáticos no Active Directory local, você precisará ser um administrador do Active Directory e do AD FS (se aplicável).

Para obter mais detalhes sobre como resolver os possíveis problemas com a associação híbrida, consulte [Solucionar problemas de Associação Híbrida](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) para configurar dispositivos híbridos associados ao Azure Active Directory e Gerenciar Dispositivos usando o portal do Azure Ad, consulte [Configurar dispositivos híbridos associados ao Azure Active Directory (associados ao domínio local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gerenciar dispositivos usando o portal do Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Para resolver problemas comuns com o ingresso no Azure Active Directory híbrido (AD), confira [perguntas frequentes sobre ingresso no Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
