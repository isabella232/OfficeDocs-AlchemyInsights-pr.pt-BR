---
title: Solucionar problemas com inscrevendo dispositivos com Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655871"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="c2475-102">Solucionar problemas com inscrevendo dispositivos com Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c2475-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="c2475-103">Revise os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="c2475-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c2475-104">Alguns problemas comuns e as etapas de solução:</span><span class="sxs-lookup"><span data-stu-id="c2475-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="c2475-p101">**Dispositivo não criptografadas erro no Portal da empresa:** Versões mais recentes do Android, particularmente começando com a versão 7.0, exigem uma senha de inicialização para certificar-se de que seu dispositivo totalmente é criptografado. Soluções comuns são habilitar um pin de inicialização ou totalmente criptografar o dispositivo. Revise [Este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="c2475-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="c2475-p102">**Dispositivos não poderão fazer check in no serviço Intune ou exibir como "Não íntegra" no console de administração do Intune:** Alguns 4.4 Samsung e 5,5 dispositivos não poderão verificar no serviço. Existem 3 possíveis soluções para esse problema:</span><span class="sxs-lookup"><span data-stu-id="c2475-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="c2475-110">Abra manualmente o aplicativo Intune Portal da empresa, que iniciará automaticamente uma sincronização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c2475-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="c2475-111">Atualize o dispositivo para Android 6.0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="c2475-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="c2475-p103">Desabilite o Gerenciador de inteligente Samsung do gerenciamento do Portal da empresa Intune. Examine [Este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e soluções.</span><span class="sxs-lookup"><span data-stu-id="c2475-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="c2475-p104">**Inválido para tipo de licença do usuário** ou **erro de nome de usuário não reconhecido:** o usuário precisa ter uma licença Intune ou EMS. Examine esses documentos para atribuir uma licença por meio: portal do Centro de administração do Office ou do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c2475-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="c2475-116">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="c2475-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c2475-p105">Use [Intune Portal de solução de problemas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Revise [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="c2475-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c2475-119">Revise [Este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para obter uma lista dos erros comuns que impedem o registro e resoluções para cada um.</span><span class="sxs-lookup"><span data-stu-id="c2475-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="c2475-120">[Saiba como inscrever-se no Microsoft Intune dispositivos com Android](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="c2475-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

