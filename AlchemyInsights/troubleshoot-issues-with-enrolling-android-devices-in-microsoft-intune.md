---
title: Solucionar problemas com o registro de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008066"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Solucionar problemas com o registro de dispositivos Android no Microsoft Intune

Revise os recursos listados abaixo para resolver seu problema agora.
  
Alguns problemas comuns e etapas de resolução:
  
 **Erro de dispositivo não criptografado Portal da Empresa:** Versões mais recentes do Android, particularmente começando com v7.0, exigem uma senha de inicialização para garantir que seu dispositivo seja totalmente criptografado. As soluções comuns são habilitar um pino de inicialização ou criptografar totalmente o dispositivo. Revise [este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.
  
 **Os dispositivos não conseguem fazer check-in com o serviço do Intune ou são exibidos como "Não Áveis" no console de administração do Intune:** Alguns dispositivos Samsung 4.4 e 5.5 podem não fazer check-in no serviço. Há três soluções possíveis para esse problema:
  
1. Abra manualmente o aplicativo Portal da Empresa do Intune, que iniciará automaticamente uma sincronização de dispositivo.

2. Atualize o dispositivo para Android 6.0 ou superior.

3. Desabilite o Gerenciador Inteligente da Samsung de gerenciar o Portal da Empresa do Intune. Revise [este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e resoluções.

 **Tipo de Licença de** Usuário Erro inválido ou nome de usuário não **reconhecido:** o usuário precisa ter uma licença do Intune ou EMS. Revise esses documentos para atribuir uma licença por meio de: Office Admin Center ou portal do Azure.
  
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

2. Revise [este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) para ver uma lista de erros comuns que impedem o registro e as resoluções de cada um.

3. [Saiba como registrar dispositivos Android em Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
