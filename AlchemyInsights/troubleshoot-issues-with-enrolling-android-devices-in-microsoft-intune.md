---
title: Solucionar problemas com inscrevendo dispositivos com Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655871"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Solucionar problemas com inscrevendo dispositivos com Android no Microsoft Intune

Revise os recursos listados abaixo para resolver o problema agora.
  
Alguns problemas comuns e as etapas de solução:
  
 **Dispositivo não criptografadas erro no Portal da empresa:** Versões mais recentes do Android, particularmente começando com a versão 7.0, exigem uma senha de inicialização para certificar-se de que seu dispositivo totalmente é criptografado. Soluções comuns são habilitar um pin de inicialização ou totalmente criptografar o dispositivo. Revise [Este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações. 
  
 **Dispositivos não poderão fazer check in no serviço Intune ou exibir como "Não íntegra" no console de administração do Intune:** Alguns 4.4 Samsung e 5,5 dispositivos não poderão verificar no serviço. Existem 3 possíveis soluções para esse problema: 
  
1. Abra manualmente o aplicativo Intune Portal da empresa, que iniciará automaticamente uma sincronização de dispositivo.
    
2. Atualize o dispositivo para Android 6.0 ou superior.
    
3. Desabilite o Gerenciador de inteligente Samsung do gerenciamento do Portal da empresa Intune. Examine [Este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e soluções. 
    
 **Inválido para tipo de licença do usuário** ou **erro de nome de usuário não reconhecido:** o usuário precisa ter uma licença Intune ou EMS. Examine esses documentos para atribuir uma licença por meio: portal do Centro de administração do Office ou do Windows Azure. 
  
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes. 
    
2. Revise [Este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um. 
    
3. [Saiba como inscrever-se no Microsoft Intune dispositivos com Android](https://docs.microsoft.com/intune/android-enroll).
    

