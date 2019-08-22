---
title: Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500059"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune

Confira os recursos listados abaixo para resolver seu problema agora.
  
Alguns problemas comuns e etapas de resolução:
  
 **Erro de dispositivo não criptografado no portal da empresa:** As versões mais recentes do Android, principalmente a partir do v 7.0, exigem uma senha de inicialização para garantir que o dispositivo seja totalmente criptografado. Soluções comuns são habilitar um PIN de inicialização ou criptografar completamente o dispositivo. Revise [este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.
  
 **Os dispositivos falham ao fazer check-in com o serviço do Intune ou exibir como "não íntegro" no console de administração do Intune:** Alguns dispositivos Samsung 4,4 e 5,5 podem não verificar no serviço. Há três soluções possíveis para esse problema:
  
1. Abra manualmente o aplicativo portal da empresa do Intune, que iniciará automaticamente uma sincronização de dispositivo.

2. Atualize o dispositivo para Android 6,0 ou superior.

3. Desabilitar o Samsung Smart Manager para gerenciar o portal da empresa do Intune. Revise [este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e resoluções.

 Erro de **tipo de licença de usuário inválido** ou **nome de usuário não reconhecido:** o usuário precisa receber uma licença do Intune ou EMS. Revise esses documentos para atribuir uma licença por meio de: centro de administração do Office ou portal do Azure.
  
Recursos adicionais para ajudar a resolver o problema:
  
1. Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

2. Revise [este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um.

3. [Saiba como registrar dispositivos Android no Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
