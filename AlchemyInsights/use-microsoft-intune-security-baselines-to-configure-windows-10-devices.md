---
title: Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641613"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="55cd9-102">Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="55cd9-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="55cd9-103">As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="55cd9-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="55cd9-104">As linhas de base de segurança são grupos pré-configurados das configurações do Windows usados para aplicar um grupo conhecido de configurações e valores padrão recomendados por equipes de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="55cd9-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="55cd9-105">Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55cd9-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="55cd9-106">Quando você implanta linhas de base de segurança para grupos de usuários ou dispositivos, as configurações são aplicadas aos dispositivos que são executados no Windows 10 ou em versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="55cd9-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="55cd9-107">Por exemplo, a linha de base de segurança (1) de gerenciamento de dispositivo móvel da Microsoft (MDM) habilita o BitLocker para unidades removíveis, (2) requer a senha para desbloquear um dispositivo e (3) desabilita a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="55cd9-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="55cd9-108">Quando um valor padrão não funciona para seu ambiente, você pode personalizar a linha de base para aplicar as configurações de que precisa.</span><span class="sxs-lookup"><span data-stu-id="55cd9-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="55cd9-109">As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55cd9-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="55cd9-110">Veja a seguir alguns benefícios dessa funcionalidade:</span><span class="sxs-lookup"><span data-stu-id="55cd9-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="55cd9-111">Uma linha de base de segurança inclui as práticas recomendadas e recomendações para as configurações que afetam a segurança.</span><span class="sxs-lookup"><span data-stu-id="55cd9-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="55cd9-112">Como os parceiros do Intune com a equipe de segurança do Windows que cria linhas de base para políticas de grupo, essas recomendações têm base em orientações sólidas e em uma vasta experiência.</span><span class="sxs-lookup"><span data-stu-id="55cd9-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="55cd9-113">Se você não tiver certeza sobre onde começar no Intune, as linhas de base de segurança o ajudarão a criar e implantar rapidamente um perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="55cd9-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="55cd9-114">Se você estiver usando uma política de grupo no momento, migrar para o Intune para fins de gerenciamento é muito mais fácil com linhas de base de segurança, porque essas linhas de base de segurança são internas no Intune e incluem recursos de ponta para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="55cd9-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="55cd9-115">Para saber mais, consulte [as linhas de base de segurança do Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e o [Gerenciamento de dispositivos móveis](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="55cd9-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>