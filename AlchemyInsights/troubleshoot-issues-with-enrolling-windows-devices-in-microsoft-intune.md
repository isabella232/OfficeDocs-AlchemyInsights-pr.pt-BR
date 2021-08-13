---
title: Solucionar problemas com o registro Windows dispositivos Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981029"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas com o registro Windows dispositivos Microsoft Intune

Revise os recursos listados abaixo para resolver seu problema agora.
  
Algumas mensagens de erro comuns e etapas de resolução:
  
 **O software não pode ser instalado, 0x80cf4017:** Seu certificado de conta expirou. Baixe o pacote de software cliente do computador no Console de Administração do Intune. Revise esta documentação para obter mais informações.
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
-  O usuário tem mais dispositivos inscritos do que o limite do dispositivo. Revise esses documentos para [remover um dispositivo ou](https://docs.microsoft.com/intune/devices-wipe) alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Os usuários podem ingressar dispositivos no Azure AD" está definido como "nenhum". De defini-lo como todos ou selecionar usuários. Revise [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.

-  O dispositivo já está inscrito por outro usuário. Se esse for o caso, remova o dispositivo do console do Azure Intune ou desemrolle manualmente o dispositivo antes de tentar novamente.

-  O dispositivo é Windows 10 Home. Somente Windows 10 Pro, Educação e Enterprise SKUs podem ingressar Azure Active Directory.

Recursos adicionais para ajudar a resolver o problema:
  
-  Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

-  Veja estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um deles: [Guia de Solução de Problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento de Solução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Saiba como registrar Windows dispositivos em Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
