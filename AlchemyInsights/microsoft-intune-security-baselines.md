---
title: Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783150"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="1c93d-102">Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos</span><span class="sxs-lookup"><span data-stu-id="1c93d-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="1c93d-103">As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1c93d-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1c93d-104">As linhas de base de segurança Windows configurações pré-configuradas usadas para aplicar um grupo conhecido de configurações e valores padrão recomendados pelas equipes de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="1c93d-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1c93d-105">Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c93d-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1c93d-106">Quando você implanta linhas de base de segurança em grupos de usuários ou dispositivos, as configurações são aplicadas a dispositivos que são executados Windows 10 ou posteriores.</span><span class="sxs-lookup"><span data-stu-id="1c93d-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="1c93d-107">Por exemplo, a linha de base de segurança de gerenciamento de dispositivo móvel (MDM) da Microsoft habilita automaticamente o BitLocker para unidades removíveis, exige a senha para desbloquear um dispositivo e desabilita a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="1c93d-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="1c93d-108">Quando um valor padrão não funciona para seu ambiente, você pode personalizar a linha de base para aplicar as configurações de que precisa.</span><span class="sxs-lookup"><span data-stu-id="1c93d-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1c93d-109">As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1c93d-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1c93d-110">Uma linha de base de segurança inclui as práticas recomendadas e recomendações para as configurações que afetam a segurança.</span><span class="sxs-lookup"><span data-stu-id="1c93d-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1c93d-111">O Intune é parceiro da equipe de segurança Windows que cria linhas de base para políticas de grupo, portanto, essas recomendações se baseiam em orientações sólidas e em uma experiência extensa.</span><span class="sxs-lookup"><span data-stu-id="1c93d-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="1c93d-112">Se você for novo no Intune e não tiver certeza de onde começar, as linhas de base de segurança ajudarão você a criar e implantar rapidamente um perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="1c93d-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="1c93d-113">Se você usa atualmente uma política de grupo, migrar para o Intune para fins de gerenciamento é muito mais fácil com as linhas de base de segurança porque elas são internas no Intune e incluem recursos de gerenciamento de borda.</span><span class="sxs-lookup"><span data-stu-id="1c93d-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="1c93d-114">Para saber mais, consulte [Windows de segurança](/windows/security/threat-protection/windows-security-baselines) e gerenciamento de [dispositivos móveis.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="1c93d-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

