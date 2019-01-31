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
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661497"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas com inscrevendo dispositivos do Windows no Microsoft Intune

Revise os recursos listados abaixo para resolver o problema agora. 
  
Algumas mensagens de erro comuns e as etapas de solução:
  
 **Não pode ser instalado o software, 0x80cf4017:** Seu certificado de conta expirou. Novamente, baixe o pacote de software de cliente PC no Console de administração do Intune. Revise esta documentação para obter mais informações. 
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários: 
  
1. O usuário tem mais dispositivos inscritos que o limite do dispositivo. Examine esses documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Os usuários podem ingressar dispositivos para o Windows Azure AD" é definido como "none". Defini-la a todos ou selecione os usuários. Revise [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações. 
    
3. O dispositivo já está inscrito por outro usuário. Se for esse o caso, remova o dispositivo do console do Windows Azure Intune ou manualmente não registrar o dispositivo antes de tentar novamente.
    
4. O dispositivo é 10 Windows Home. Somente Windows 10 Pro, treinamento e Enterprise SKUs podem ingressar Azure Active Directory.
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes. 
    
2. Examine esses documentos para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um: [guia de solução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [doc de solução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Aprenda a registrar os dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

