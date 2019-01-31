---
title: Solucionar problemas com inscrevendo dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658427"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Solucionar problemas com inscrevendo dispositivos iOS no Microsoft Intune

Revise os recursos listados abaixo para resolver o problema agora. 
  
Algumas mensagens de erro comuns e as etapas de solução:
  
- **Limite do dispositivo atingido** O usuário tem mais dispositivos inscritos que o limite do dispositivo. Examine esses documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Este serviço não é suportado. Nenhuma diretiva de registro:** serviço de notificação por Push da Apple (APNS) precisa ser configurado ou renovado. Revise [Este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazer isso. 
    
- **Tipo de licença de usuário inválido ou nome de usuário não reconhecida:** O usuário precisa ter uma licença Intune ou EMS. Examine esses documentos para atribuir uma licença por meio: [Centro de administração do Office](https://docs.microsoft.com/intune/licenses-assign) ou [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes. 
    
2. Examine esses documentos para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um: [guia de solução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [doc de solução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Aprenda a registrar dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

