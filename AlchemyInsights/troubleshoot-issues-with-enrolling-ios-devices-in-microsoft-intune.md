---
title: Solucionar problemas com o registro de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823451"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Solucionar problemas com o registro de dispositivos iOS no Microsoft Intune

Revise os recursos listados abaixo para resolver seu problema agora. 
  
Algumas mensagens de erro comuns e etapas de resolução:
  
- **Device Cap Reached** O usuário tem mais dispositivos inscritos do que o limite do dispositivo. Revise esses documentos para [remover um dispositivo ou](https://docs.microsoft.com/intune/devices-wipe) alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Este Serviço não tem suporte. Sem Política de Registro:** o Serviço de Notificação por Push da Apple (APNS) precisa ser configurado ou renovado. Revise [este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazer isso. 
    
- **Tipo de licença de usuário inválido ou nome de usuário não reconhecido:** O usuário precisa ter uma licença do Intune ou EMS. Revise esses documentos para atribuir uma licença por: [Centro de Administração do Office](https://docs.microsoft.com/intune/licenses-assign) ou portal do [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes. 
    
2. Veja estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um deles: [Guia de Solução de Problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento de Solução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Saiba como registrar dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

