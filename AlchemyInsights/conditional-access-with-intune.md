---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807647"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="37a2a-102">Acesso condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="37a2a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="37a2a-103">O uso do  **acesso condicional**  com o Intune requer três etapas:</span><span class="sxs-lookup"><span data-stu-id="37a2a-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="37a2a-104">Crie uma  **política de conformidade**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [Ios](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="37a2a-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="37a2a-105">Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade.</span><span class="sxs-lookup"><span data-stu-id="37a2a-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="37a2a-106">Criar uma **política de acesso condicional**  que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="37a2a-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="37a2a-107">[Por exemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  um dispositivo deve estar em conformidade antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="37a2a-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="37a2a-108">Verifique se as políticas de **conformidade**  e  **as políticas de acesso condicional**  estão direcionadas para os grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="37a2a-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="37a2a-109">Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="37a2a-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="37a2a-110">**Links úteis:**</span><span class="sxs-lookup"><span data-stu-id="37a2a-110">**Helpful links:**</span></span>

[<span data-ttu-id="37a2a-111">Visão geral de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="37a2a-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="37a2a-112">Solucionando problemas de autoridade de certificação</span><span class="sxs-lookup"><span data-stu-id="37a2a-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="37a2a-113">Política de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="37a2a-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="37a2a-114">Para proteger o email (Exchange Online) do acesso por dispositivos não compatíveis, ambos os documentos devem ser seguidos:</span><span class="sxs-lookup"><span data-stu-id="37a2a-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="37a2a-115">Proteger o acesso de email de dispositivos usando EAS</span><span class="sxs-lookup"><span data-stu-id="37a2a-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="37a2a-116">Proteger o acesso de email de dispositivos usando clientes de autenticação modernos, como o Outlook</span><span class="sxs-lookup"><span data-stu-id="37a2a-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)