---
title: Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689942"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="0cf77-102">Solucionar problemas com a inscrição de dispositivos Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0cf77-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="0cf77-103">Confira os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="0cf77-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0cf77-104">Alguns problemas comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="0cf77-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="0cf77-105">**Erro de dispositivo não criptografado no portal da empresa:** As versões mais recentes do Android, principalmente a partir do v 7.0, exigem uma senha de inicialização para garantir que o dispositivo seja totalmente criptografado.</span><span class="sxs-lookup"><span data-stu-id="0cf77-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="0cf77-106">Soluções comuns são habilitar um PIN de inicialização ou criptografar completamente o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cf77-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="0cf77-107">Revise [este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="0cf77-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="0cf77-108">**Os dispositivos falham ao fazer check-in com o serviço do Intune ou exibir como "não íntegro" no console de administração do Intune:** Alguns dispositivos Samsung 4,4 e 5,5 podem não verificar no serviço.</span><span class="sxs-lookup"><span data-stu-id="0cf77-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="0cf77-109">Há três soluções possíveis para esse problema:</span><span class="sxs-lookup"><span data-stu-id="0cf77-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="0cf77-110">Abra manualmente o aplicativo portal da empresa do Intune, que iniciará automaticamente uma sincronização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cf77-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="0cf77-111">Atualize o dispositivo para Android 6,0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="0cf77-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="0cf77-112">Desabilitar o Samsung Smart Manager para gerenciar o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="0cf77-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="0cf77-113">Revise [este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre esses problemas e resoluções.</span><span class="sxs-lookup"><span data-stu-id="0cf77-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="0cf77-114">Erro de **tipo de licença de usuário inválido** ou **nome de usuário não reconhecido:** o usuário precisa receber uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="0cf77-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="0cf77-115">Revise esses documentos para atribuir uma licença por meio de: centro de administração do Office ou portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0cf77-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="0cf77-116">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="0cf77-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0cf77-117">Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="0cf77-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0cf77-118">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="0cf77-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="0cf77-119">Revise [este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um.</span><span class="sxs-lookup"><span data-stu-id="0cf77-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="0cf77-120">[Saiba como registrar dispositivos Android no Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="0cf77-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
