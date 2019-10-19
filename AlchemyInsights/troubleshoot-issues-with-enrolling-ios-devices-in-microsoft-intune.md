---
title: Solucionar problemas com a inscrição de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506869"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="62543-102">Solucionar problemas com a inscrição de dispositivos iOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62543-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="62543-103">Confira os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="62543-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="62543-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="62543-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="62543-105">**Limite do dispositivo atingido** O usuário tem mais dispositivos registrados que o limite de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="62543-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="62543-106">Revise esses documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite de dispositivos](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="62543-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="62543-107">**Não há suporte para esse serviço. Nenhuma política de registro:** o Apple Push Notification Service (APNS) precisa ser configurado ou renovado.</span><span class="sxs-lookup"><span data-stu-id="62543-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="62543-108">Revise [este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="62543-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="62543-109">**Tipo de licença de usuário inválido ou nome de usuário não reconhecido:** O usuário precisa receber uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="62543-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="62543-110">Revise esses documentos para atribuir uma licença por meio de: [centro de administração do Office](https://docs.microsoft.com/intune/licenses-assign) ou [portal do Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="62543-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="62543-111">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="62543-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="62543-112">Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="62543-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="62543-113">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="62543-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="62543-114">Revise estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada: [Guia de solução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e doc de solução de [problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="62543-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="62543-115">[Saiba como registrar dispositivos IOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="62543-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

