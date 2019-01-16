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
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="7a7df-102">Solucionar problemas com inscrevendo dispositivos do Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7a7df-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="7a7df-103">Revise os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="7a7df-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="7a7df-104">Algumas mensagens de erro comuns e as etapas de solução:</span><span class="sxs-lookup"><span data-stu-id="7a7df-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="7a7df-p101">**Não pode ser instalado o software, 0x80cf4017:** Seu certificado de conta expirou. Novamente, baixe o pacote de software de cliente PC no Console de administração do Intune. Revise esta documentação para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7a7df-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="7a7df-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="7a7df-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="7a7df-p102">O usuário tem mais dispositivos inscritos que o limite do dispositivo. Examine esses documentos para [Remover um dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="7a7df-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="7a7df-p103">"Os usuários podem ingressar dispositivos para o Windows Azure AD" é definido como "none". Defini-la a todos ou selecione os usuários. Revise [esta documentação](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7a7df-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="7a7df-p104">O dispositivo já está inscrito por outro usuário. Se for esse o caso, remova o dispositivo do console do Windows Azure Intune ou manualmente não registrar o dispositivo antes de tentar novamente.</span><span class="sxs-lookup"><span data-stu-id="7a7df-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="7a7df-p105">O dispositivo é 10 Windows Home. Somente Windows 10 Pro, treinamento e Enterprise SKUs podem ingressar Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a7df-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="7a7df-118">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="7a7df-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7a7df-p106">Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="7a7df-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7a7df-121">Examine esses documentos para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um: [guia de solução de problemas](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [doc de solução de problemas](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="7a7df-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="7a7df-122">[Aprenda a registrar os dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="7a7df-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

