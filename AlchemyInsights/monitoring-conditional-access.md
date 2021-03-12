---
title: Monitoramento do Acesso Condicional
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708662"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="f52a8-102">Monitorando o acesso condicional para o Exchange</span><span class="sxs-lookup"><span data-stu-id="f52a8-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="f52a8-103">Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="f52a8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f52a8-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="f52a8-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="f52a8-105">Se presume-se que o dispositivo está inscrito, aconselha o usuário a ir até o aplicativo Portal da Empresa e verificar se ele aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="f52a8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f52a8-106">Se não for, o usuário deverá registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f52a8-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="f52a8-107">No portal do Azure, acesse Intune > Conformidade com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f52a8-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="f52a8-108">Em Monitorar, clique em Conformidade com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f52a8-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="f52a8-109">Exibir o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="f52a8-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="f52a8-110">No portal do Azure, acesse Intune > Conformidade com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f52a8-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="f52a8-111">Em Gerenciar, clique em Políticas.</span><span class="sxs-lookup"><span data-stu-id="f52a8-111">Under Manage, click Policies.</span></span> <span data-ttu-id="f52a8-112">Na lista de políticas de conformidade, verifique se um perfil está atribuído ao dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f52a8-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f52a8-113">Se nenhum perfil for atribuído, o Intune não poderá confirmar o status de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f52a8-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="f52a8-114">Edite a atribuição de acesso condicional do usuário.</span><span class="sxs-lookup"><span data-stu-id="f52a8-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="f52a8-115">No portal do Azure, acesse Políticas de acesso condicional do **Intune.**  >    >  </span><span class="sxs-lookup"><span data-stu-id="f52a8-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="f52a8-116">Selecione uma política na lista.</span><span class="sxs-lookup"><span data-stu-id="f52a8-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="f52a8-117">Clique em Usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="f52a8-117">Click Users and groups.</span></span>
4. <span data-ttu-id="f52a8-118">Para direcionar uma determinada política para alguém, adicione-a à lista Incluir.</span><span class="sxs-lookup"><span data-stu-id="f52a8-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="f52a8-119">Para garantir que uma pessoa seja omitida da política, adicione-a à lista Excluir.</span><span class="sxs-lookup"><span data-stu-id="f52a8-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="f52a8-120">Links úteis:</span><span class="sxs-lookup"><span data-stu-id="f52a8-120">Helpful links:</span></span>

[<span data-ttu-id="f52a8-121">Visão geral da conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f52a8-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f52a8-122">Solução de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="f52a8-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f52a8-123">Política de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="f52a8-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="f52a8-124">Monitorando a conformidade do dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="f52a8-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="f52a8-125">Observação: essas etapas só são úteis na solução de problemas do recurso do Azure Active Directory Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="f52a8-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="f52a8-126">Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com a política do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f52a8-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="f52a8-127">Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [aqui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="f52a8-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
