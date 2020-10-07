---
title: Implantação do aplicativo Win32 do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366489"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="ea8f3-102">Implantação do aplicativo Win32 do Intune</span><span class="sxs-lookup"><span data-stu-id="ea8f3-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="ea8f3-103">O Microsoft Intune permite aplicativos Win32, incluindo, mas não se limitando a MSI, e .EXE para ser implantado em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="ea8f3-104">O mecanismo de implantação usado exige que a extensão de gerenciamento do Intune (IME) esteja presente no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="ea8f3-105">O IME será instalado automaticamente como resultado da implantação de um script do PowerShell ou do aplicativo Win32 em um usuário/dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="ea8f3-106">Há também um conjunto de pré-requisitos que devem ser atendidos para a implantação de aplicativos Win32 que incluem:</span><span class="sxs-lookup"><span data-stu-id="ea8f3-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="ea8f3-107">Plataformas suportadas: Windows 10 versão 1607 ou posterior (versões Enterprise, Pro e Education).</span><span class="sxs-lookup"><span data-stu-id="ea8f3-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="ea8f3-108">Arquiteturas suportadas: x86 e x64.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="ea8f3-109">Gerenciamento de dispositivo: o AAD ingressou e se registrou automaticamente (incluindo a política de grupo e de domínios híbridos).</span><span class="sxs-lookup"><span data-stu-id="ea8f3-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="ea8f3-110">Formato de pacote de aplicativo: o arquivo **intunewin** preparado pela [ferramenta de preparação de conteúdo Win32 da Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="ea8f3-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="ea8f3-111">Limitações:</span><span class="sxs-lookup"><span data-stu-id="ea8f3-111">Limitations:</span></span>
    - <span data-ttu-id="ea8f3-112">Tamanho máximo: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="ea8f3-113">Arquitetura sem suporte: ARMs.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="ea8f3-114">Examine o documento "[Adicionar, atribuir e monitorar um aplicativo Win32 no Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para saber mais sobre essas etapas.</span><span class="sxs-lookup"><span data-stu-id="ea8f3-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="ea8f3-115">Detalhes de solução de problemas de implantação de aplicativos no Windows, incluindo aplicativos Win32, podem ser analisados nos seguintes documentos</span><span class="sxs-lookup"><span data-stu-id="ea8f3-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="ea8f3-116">Solucionar problemas de instalação do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea8f3-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="ea8f3-117">Solucionar problemas de aplicativos Win32</span><span class="sxs-lookup"><span data-stu-id="ea8f3-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)