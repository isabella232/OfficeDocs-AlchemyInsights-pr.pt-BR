---
title: Solucionar problemas com inscrevendo dispositivos do Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275157"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas com inscrevendo dispositivos do Windows no Microsoft Intune

Revise os recursos listados abaixo para resolver o problema agora. 
  
Algumas mensagens de erro comuns e as etapas de solução:
  
 **Não pode ser instalado o software, 0x80cf4017:** Seu certificado de conta expirou. Novamente, baixe o pacote de software de cliente PC no Console de administração do Intune. Revise esta documentação para obter mais informações. 
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários: 
  
1. O usuário tem mais dispositivos inscritos que o limite do dispositivo. Examine esses documentos para [Remover um dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Os usuários podem ingressar dispositivos para o Windows Azure AD" é definido como "none". Defini-la a todos ou selecione os usuários. Revise [esta documentação](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações. 
    
3. O dispositivo já está inscrito por outro usuário. Se for esse o caso, remova o dispositivo do console do Windows Azure Intune ou manualmente não registrar o dispositivo antes de tentar novamente.
    
4. O dispositivo é 10 Windows Home. Somente Windows 10 Pro, treinamento e Enterprise SKUs podem ingressar Azure Active Directory.
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) para obter mais detalhes. 
    
2. Examine esses documentos para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um: [guia de solução de problemas](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [doc de solução de problemas](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Aprenda a registrar os dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

