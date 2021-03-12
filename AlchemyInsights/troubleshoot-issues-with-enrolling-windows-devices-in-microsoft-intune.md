---
title: Solucionar problemas com o registro de dispositivos Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708878"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="4e0ae-102">Solucionar problemas com o registro de dispositivos Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e0ae-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="4e0ae-103">Revise os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="4e0ae-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="4e0ae-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="4e0ae-105">**O software não pode ser instalado, 0x80cf4017:** Seu certificado de conta expirou.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="4e0ae-106">Baixe o pacote de software cliente do computador no Console de Administração do Intune.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="4e0ae-107">Revise esta documentação para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="4e0ae-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="4e0ae-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="4e0ae-109">O usuário tem mais dispositivos inscritos do que o limite do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4e0ae-110">Revise esses documentos para [remover um dispositivo ou](https://docs.microsoft.com/intune/devices-wipe) alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="4e0ae-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="4e0ae-111">"Os usuários podem ingressar dispositivos no Azure AD" está definido como "nenhum".</span><span class="sxs-lookup"><span data-stu-id="4e0ae-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="4e0ae-112">De defini-lo como todos ou selecionar usuários.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-112">Set it to all or select users.</span></span> <span data-ttu-id="4e0ae-113">Revise [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="4e0ae-114">O dispositivo já está inscrito por outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="4e0ae-115">Se esse for o caso, remova o dispositivo do console do Azure Intune ou desemrolle manualmente o dispositivo antes de tentar novamente.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="4e0ae-116">O dispositivo é o Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="4e0ae-117">Somente os SKUs Do Windows 10 Pro, Education e Enterprise podem ingressar no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="4e0ae-118">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="4e0ae-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="4e0ae-119">Use [o Portal de Solução de Problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4e0ae-120">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="4e0ae-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="4e0ae-121">Veja estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada um deles: [Guia de Solução de Problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento de Solução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4e0ae-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="4e0ae-122">[Saiba como registrar dispositivos Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="4e0ae-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
