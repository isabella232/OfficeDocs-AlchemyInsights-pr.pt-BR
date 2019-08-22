---
title: Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500059"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9b9c4-102">Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9b9c4-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9b9c4-103">Confira os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9b9c4-104">Alguns problemas comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="9b9c4-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9b9c4-105">**Erro de dispositivo não criptografado no portal da empresa:** As versões mais recentes do Android, principalmente a partir do v 7.0, exigem uma senha de inicialização para garantir que o dispositivo seja totalmente criptografado.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="9b9c4-106">Soluções comuns são habilitar um PIN de inicialização ou criptografar completamente o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="9b9c4-107">Revise [este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="9b9c4-108">**Os dispositivos falham ao fazer check-in com o serviço do Intune ou exibir como "não íntegro" no console de administração do Intune:** Alguns dispositivos Samsung 4,4 e 5,5 podem não verificar no serviço.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="9b9c4-109">Há três soluções possíveis para esse problema:</span><span class="sxs-lookup"><span data-stu-id="9b9c4-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="9b9c4-110">Abra manualmente o aplicativo portal da empresa do Intune, que iniciará automaticamente uma sincronização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="9b9c4-111">Atualize o dispositivo para Android 6,0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="9b9c4-112">Desabilitar o Samsung Smart Manager para gerenciar o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="9b9c4-113">Revise [este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e resoluções.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="9b9c4-114">Erro de **tipo de licença de usuário inválido** ou **nome de usuário não reconhecido:** o usuário precisa receber uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9b9c4-115">Revise esses documentos para atribuir uma licença por meio de: centro de administração do Office ou portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="9b9c4-116">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="9b9c4-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9b9c4-117">Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9b9c4-118">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9b9c4-119">Revise [este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um.</span><span class="sxs-lookup"><span data-stu-id="9b9c4-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="9b9c4-120">[Saiba como registrar dispositivos Android no Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="9b9c4-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
