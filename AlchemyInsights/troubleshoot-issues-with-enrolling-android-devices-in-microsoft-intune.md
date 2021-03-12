---
title: Solucionar problemas com o registro de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708986"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="265c4-102">Solucionar problemas com o registro de dispositivos Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="265c4-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="265c4-103">Revise os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="265c4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="265c4-104">Alguns problemas comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="265c4-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="265c4-105">**Erro de dispositivo não criptografado no Portal da Empresa:** Versões mais recentes do Android, particularmente começando com v7.0, exigem uma senha de inicialização para garantir que seu dispositivo seja totalmente criptografado.</span><span class="sxs-lookup"><span data-stu-id="265c4-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="265c4-106">As soluções comuns são habilitar um pino de inicialização ou criptografar totalmente o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="265c4-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="265c4-107">Revise [este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="265c4-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="265c4-108">**Os dispositivos não conseguem fazer check-in com o serviço do Intune ou são exibidos como "Não Áveis" no console de administração do Intune:** Alguns dispositivos Samsung 4.4 e 5.5 podem não fazer check-in no serviço.</span><span class="sxs-lookup"><span data-stu-id="265c4-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="265c4-109">Há três soluções possíveis para esse problema:</span><span class="sxs-lookup"><span data-stu-id="265c4-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="265c4-110">Abra manualmente o aplicativo Portal da Empresa do Intune, que iniciará automaticamente uma sincronização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="265c4-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="265c4-111">Atualize o dispositivo para Android 6.0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="265c4-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="265c4-112">Desabilite o Gerenciador Inteligente da Samsung do gerenciamento do Portal da Empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="265c4-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="265c4-113">Revise [este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e resoluções.</span><span class="sxs-lookup"><span data-stu-id="265c4-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="265c4-114">**Tipo de Licença de** Usuário Erro inválido ou nome de usuário não **reconhecido:** o usuário precisa ter uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="265c4-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="265c4-115">Revise esses documentos para atribuir uma licença por meio: Centro de Administração do Office ou portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="265c4-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="265c4-116">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="265c4-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="265c4-117">Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="265c4-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="265c4-118">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="265c4-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="265c4-119">Revise [este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) para ver uma lista de erros comuns que impedem o registro e as resoluções de cada um.</span><span class="sxs-lookup"><span data-stu-id="265c4-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="265c4-120">[Saiba como registrar dispositivos Android no Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="265c4-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
