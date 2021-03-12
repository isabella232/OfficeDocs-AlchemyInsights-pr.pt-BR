---
title: Solucionar problemas com o registro de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708950"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="86c07-102">Solucionar problemas com o registro de dispositivos iOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="86c07-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="86c07-103">Revise os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="86c07-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="86c07-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="86c07-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="86c07-105">**Device Cap Reached** O usuário tem mais dispositivos inscritos do que o limite do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86c07-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="86c07-106">Revise esses documentos para [remover um dispositivo ou](https://docs.microsoft.com/intune/devices-wipe) alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="86c07-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="86c07-107">**Este Serviço não tem suporte. Sem Política de Registro:** o Serviço de Notificação por Push da Apple (APNS) precisa ser configurado ou renovado.</span><span class="sxs-lookup"><span data-stu-id="86c07-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="86c07-108">Revise [este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="86c07-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="86c07-109">**Tipo de licença de usuário inválido ou nome de usuário não reconhecido:** O usuário precisa ter uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="86c07-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="86c07-110">Revise esses documentos para atribuir uma licença por: [Centro de Administração do Office](https://docs.microsoft.com/intune/licenses-assign) ou portal do [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="86c07-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="86c07-111">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="86c07-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="86c07-112">Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="86c07-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="86c07-113">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="86c07-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="86c07-114">Veja estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um deles: [Guia de Solução de Problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento de Solução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="86c07-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="86c07-115">[Saiba como registrar dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="86c07-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

