---
title: Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665820"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e41c6-102">Solucionar problemas com a inscrição de dispositivos Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e41c6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e41c6-103">Confira os recursos listados abaixo para resolver seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="e41c6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e41c6-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="e41c6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e41c6-105">**O software não pode ser instalado, 0x80cf4017:** O certificado de conta expirou.</span><span class="sxs-lookup"><span data-stu-id="e41c6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="e41c6-106">Baixe novamente o pacote de software cliente do PC no console de administração do Intune.</span><span class="sxs-lookup"><span data-stu-id="e41c6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="e41c6-107">Confira esta documentação para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e41c6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="e41c6-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="e41c6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="e41c6-109">O usuário tem mais dispositivos registrados que o limite de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e41c6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e41c6-110">Revise esses documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite de dispositivos](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e41c6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="e41c6-111">"Os usuários podem ingressar em dispositivos no Azure AD" está definido como "None".</span><span class="sxs-lookup"><span data-stu-id="e41c6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="e41c6-112">Defina-o como todos ou selecione usuários.</span><span class="sxs-lookup"><span data-stu-id="e41c6-112">Set it to all or select users.</span></span> <span data-ttu-id="e41c6-113">Confira [esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e41c6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="e41c6-114">O dispositivo já está inscrito por outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e41c6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="e41c6-115">Se esse for o caso, remova o dispositivo do console do Azure Intune ou Desregistre manualmente o dispositivo antes de tentar novamente.</span><span class="sxs-lookup"><span data-stu-id="e41c6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="e41c6-116">O dispositivo é o Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="e41c6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="e41c6-117">Somente os SKUs do Windows 10 pro, Education e Enterprise podem ingressar no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e41c6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="e41c6-118">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="e41c6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="e41c6-119">Use o [portal de solução de problemas do Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de registro.</span><span class="sxs-lookup"><span data-stu-id="e41c6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e41c6-120">Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="e41c6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="e41c6-121">Revise estes documentos para obter uma lista de erros comuns que impedem o registro e as resoluções de cada: [Guia de solução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e doc de solução de [problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e41c6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="e41c6-122">[Saiba como registrar dispositivos do Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="e41c6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
