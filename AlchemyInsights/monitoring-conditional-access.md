---
title: Monitorar o acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366416"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="04579-102">Monitorar o acesso condicional do Exchange</span><span class="sxs-lookup"><span data-stu-id="04579-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="04579-103">Os usuários direcionados ao acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="04579-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="04579-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="04579-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="04579-105">Se presumir que o dispositivo esteja inscrito, recomende que o usuário acesse o aplicativo do portal da empresa e verifique se ele aparece no portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="04579-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="04579-106">Caso contrário, o usuário deverá registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04579-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="04579-107">No portal do Azure, acesse o Intune > o dispositivo de conformidade.</span><span class="sxs-lookup"><span data-stu-id="04579-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="04579-108">Em monitorar, clique em conformidade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04579-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="04579-109">Exiba o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="04579-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="04579-110">No portal do Azure, acesse o Intune > o dispositivo de conformidade.</span><span class="sxs-lookup"><span data-stu-id="04579-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="04579-111">Em gerenciar, clique em políticas.</span><span class="sxs-lookup"><span data-stu-id="04579-111">Under Manage, click Policies.</span></span> <span data-ttu-id="04579-112">Na lista de políticas de conformidade, verifique se um perfil foi atribuído ao dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="04579-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="04579-113">Se nenhum perfil for atribuído, o Intune não conseguirá confirmar o status de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04579-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="04579-114">Edite a atribuição de acesso condicional do usuário.</span><span class="sxs-lookup"><span data-stu-id="04579-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="04579-115">No portal do Azure, acesse **Intune**  >  **Conditional access**  >  **as políticas**de acesso condicional do Intune.</span><span class="sxs-lookup"><span data-stu-id="04579-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="04579-116">Selecione uma política na lista.</span><span class="sxs-lookup"><span data-stu-id="04579-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="04579-117">Clique em usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="04579-117">Click Users and groups.</span></span>
4. <span data-ttu-id="04579-118">Para direcionar uma determinada política em alguém, adicione-a à lista de inclusões.</span><span class="sxs-lookup"><span data-stu-id="04579-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="04579-119">Para garantir que uma pessoa seja omitida da política, adicione-a à lista de exclusão.</span><span class="sxs-lookup"><span data-stu-id="04579-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="04579-120">Links úteis:</span><span class="sxs-lookup"><span data-stu-id="04579-120">Helpful links:</span></span>

[<span data-ttu-id="04579-121">Visão geral de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="04579-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="04579-122">Solucionando problemas de autoridade de certificação</span><span class="sxs-lookup"><span data-stu-id="04579-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="04579-123">Política de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="04579-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="04579-124">Monitoramento da conformidade do dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="04579-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="04579-125">Observação: estas etapas só são úteis para solucionar problemas de acesso condicional ao recurso do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04579-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="04579-126">Também é possível colocar em quarentena um dispositivo que bloqueie o acesso de email com a política do Exchange.</span><span class="sxs-lookup"><span data-stu-id="04579-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="04579-127">Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [aqui](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="04579-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
