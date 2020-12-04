---
title: Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571765"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="ac3d1-102">Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="ac3d1-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="ac3d1-103">As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ac3d1-104">As linhas de base de segurança são os grupos pré-configurados de configurações do Windows usados para aplicar um grupo conhecido de configurações e valores padrão recomendados pelas equipes de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ac3d1-105">Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ac3d1-106">Quando você implanta linhas de base de segurança para grupos de usuários ou dispositivos, as configurações são aplicadas a dispositivos executados no Windows 10 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="ac3d1-107">Por exemplo, a linha de base de segurança MDM automaticamente (1) habilita o BitLocker para unidades removíveis, (2) requer a senha para desbloquear um dispositivo e (3) desabilita a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ac3d1-108">Quando um valor padrão não funciona para seu ambiente, personalize a linha de base para aplicar as configurações de que você precisa.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ac3d1-109">As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ac3d1-110">Estes são alguns dos benefícios disso:</span><span class="sxs-lookup"><span data-stu-id="ac3d1-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="ac3d1-111">Uma linha de base de segurança inclui as práticas recomendadas e as recomendações para as configurações que afetam a segurança.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ac3d1-112">Como os parceiros do Intune com a equipe de segurança do Windows que cria linhas de base para diretivas de grupo, essas recomendações são baseadas em uma orientação sólida e uma ampla experiência.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ac3d1-113">Se você é novo no Intune e não tem certeza de onde começar, as linhas de base de segurança ajudarão você a criar e implantar rapidamente um perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ac3d1-114">Se você usa uma política de grupo no momento, a migração para o Intune para fins de gerenciamento é muito mais fácil com as linhas de base de segurança, pois elas são criadas no Intune e incluem recursos de recorte de borda para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ac3d1-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ac3d1-115">Para saber mais, confira [Windows Security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="ac3d1-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>