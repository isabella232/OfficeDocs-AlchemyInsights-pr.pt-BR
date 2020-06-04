---
title: Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665820"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune

Confira os recursos listados abaixo para resolver seu problema agora.
  
Algumas mensagens de erro comuns e etapas de resolução:
  
 **O software não pode ser instalado, 0x80cf4017:** O certificado de conta expirou. Baixe novamente o pacote de software cliente do PC no console de administração do Intune. Confira esta documentação para obter mais informações.
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
-  O usuário tem mais dispositivos registrados que o limite de dispositivos. Revise esses documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite de dispositivos](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Os usuários podem ingressar em dispositivos no Azure AD" está definido como "None". Defina-o como todos ou selecione usuários. Confira [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.

-  O dispositivo já está inscrito por outro usuário. Se esse for o caso, remova o dispositivo do console do Azure Intune ou Desregistre manualmente o dispositivo antes de tentar novamente.

-  O dispositivo é o Windows 10 Home. Somente os SKUs do Windows 10 pro, Education e Enterprise podem ingressar no Azure Active Directory.

Recursos adicionais para ajudar a resolver o problema:
  
-  Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

-  Revise estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada: [Guia de solução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e doc de solução de [problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saiba como registrar dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
