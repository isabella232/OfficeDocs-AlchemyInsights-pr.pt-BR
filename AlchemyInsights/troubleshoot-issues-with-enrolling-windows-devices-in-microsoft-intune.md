---
title: Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559613"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune

Confira os recursos listados abaixo para resolver seu problema agora.
  
Algumas mensagens de erro comuns e etapas de resolução:
  
 **O software não pode ser instalado, 0x80cf4017:** O certificado de conta expirou. Baixe novamente o pacote de software cliente do PC no console de administração do Intune. Confira esta documentação para obter mais informações.
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
1. O usuário tem mais dispositivos registrados que o limite de dispositivos. Revise esses documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite de dispositivos](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Os usuários podem ingressar em dispositivos no Azure AD" está definido como "None". Defina-o como todos ou selecione usuários. Confira [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.

3. O dispositivo já está inscrito por outro usuário. Se esse for o caso, remova o dispositivo do console do Azure Intune ou Desregistre manualmente o dispositivo antes de tentar novamente.

4. O dispositivo é o Windows 10 Home. Somente os SKUs do Windows 10 pro, Education e Enterprise podem ingressar no Azure Active Directory.

Recursos adicionais para ajudar a resolver o problema:
  
1. Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

2. Revise estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada: [Guia de solução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e doc de solução de [problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saiba como registrar dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
